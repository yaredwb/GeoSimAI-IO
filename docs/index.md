---
layout: default
title: GeoSim.AI - Coming soon...
mathjax: true
---

### A new paradigm in computational geomechanics

The ability to accomplish tasks via natural language instructions is one of the most efficient forms of interaction between humans and technology. This efficiency has been translated into practical applications, with AI-powered chatbots and voice-activated virtual assistants now allowing users to interact through natural language queries. The emergence of advanced Large Language Models (LLMs) marks a pivotal shift in this direction. With ongoing advancements in the field of AI, integrating natural language commands into sophisticated technical fields in science and engineering is becoming increasingly feasible. This paper explores the transformative potential of LLMs in enhancing numerical simulations for computational geomechanics. We investigate how AI assistants powered by LLMs can streamline the process of creating complex simulation inputs and interpreting results by translating natural language instructions into precise technical commands and scripts. This approach aims to bridge the gap between human intent and the intricate requirements of numerical modeling tools, potentially revolutionizing how researchers and engineers interact with simulation software. We present a demonstrative application to illustrate this approach, discuss implementation challenges and benefits, and explore the future prospects of AI-assisted simulation workflows. Our findings highlight the potential of this technology to significantly enhance productivity and accessibility in computational geomechanics.

### Architecture of GeoSim.AI

![GeoSimAI Architecture](/assets/figs/geosimai-architecture-v3.png)

### GeoSim.AI Interface

![GeoSimAI Interface](/assets/figs/geosimai_chat_interface_1610.png)

## Demos

### General GeoSim.AI Demos

<div class="video-gallery">
  <div class="video-scroll-container">
    <div class="video-item">
      <h3>Demo of GeoSim.AI Interface</h3>
      <iframe 
        src="https://www.youtube-nocookie.com/embed/_LprVXHBT-I?controls=1&modestbranding=1&rel=0&showinfo=0&enablejsapi=1&playlist=_LprVXHBT-I&iv_load_policy=3"
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>
  </div>
</div>

### ADONIS AI Agent Demos

<div class="video-gallery">
  <div class="video-scroll-container">
    <div class="video-item">
      <h3>Text Prompt</h3>
      <iframe 
        src="https://www.youtube-nocookie.com/embed/Te3kfmKfaSA?controls=1&modestbranding=1&rel=0&showinfo=0&enablejsapi=1&playlist=Te3kfmKfaSA&iv_load_policy=3"
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>
    <div class="video-item">
      <h3>Image + Text Prompt</h3>
      <iframe 
        src="https://www.youtube-nocookie.com/embed/Uu2_jwBv4iw?controls=1&modestbranding=1&rel=0&showinfo=0&enablejsapi=1&playlist=Uu2_jwBv4iw&iv_load_policy=3"
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>
  </div>
</div>

### HYRCAN AI Agent Demos

<div class="video-gallery">
  <div class="video-scroll-container">
    <div class="video-item">
      <h3>Text Prompt</h3>
      <iframe 
        src="https://www.youtube-nocookie.com/embed/NVIivwbvIMg?controls=1&modestbranding=1&rel=0&showinfo=0&enablejsapi=1&playlist=NVIivwbvIMg&iv_load_policy=3"
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>
    <div class="video-item">
      <h3>Image + Text Prompt</h3>
      <iframe 
        src="https://www.youtube-nocookie.com/embed/GPeWuJPa5Eg?controls=1&modestbranding=1&rel=0&showinfo=0&enablejsapi=1&playlist=GPeWuJPa5Eg&iv_load_policy=3"
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>
  </div>
</div>

### AI Agents for Commercial Software

Agents for commerical software (PLAXIS2D, PLAXIS3D, FLAC2D and FLAC3D) are only for internal use at the moment.

<style>
.video-gallery {
  width: 100%;
  margin: 0 auto;
  padding: 20px 0;
}

.video-scroll-container {
  display: grid;
  grid-auto-flow: column;
  grid-auto-columns: min-content;
  gap: 40px;
  padding: 20px 0;
  overflow-x: auto;
  scrollbar-width: thin;
  /* Remove scroll-snap to allow smooth scrolling */
}

.video-scroll-container::-webkit-scrollbar {
  height: 8px;
}

.video-scroll-container::-webkit-scrollbar-track {
  background: #f1f1f1;
  border-radius: 4px;
}

.video-scroll-container::-webkit-scrollbar-thumb {
  background: #888;
  border-radius: 4px;
}

.video-scroll-container::-webkit-scrollbar-thumb:hover {
  background: #555;
}

.video-item {
  width: calc((100vw - 120px) / 2);  /* Display 2 videos per row with gap */
  max-width: 853px;  /* Max width for YouTube's large size */
}

.video-item h3 {
  margin: 0 0 10px 0;
  font-size: 16px;
  text-align: center;
}

.video-item iframe {
  width: 100%;
  height: calc(((100vw - 120px) / 2) * 0.5625);  /* Maintain 16:9 aspect ratio */
  max-width: 853px;
  max-height: 480px;
  border: none;
  border-radius: 8px;
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

/* Responsive behavior */
@media (max-width: 1600px) {
  .video-item {
    width: calc((100vw - 80px) / 1.5);  /* Slightly larger for medium screens */
  }
  
  .video-item iframe {
    height: calc(((100vw - 80px) / 1.5) * 0.5625);
  }
}

@media (max-width: 900px) {
  .video-item {
    width: calc(100vw - 40px);  /* Full width for small screens */
  }
  
  .video-item iframe {
    height: calc((100vw - 40px) * 0.5625);
  }
}
</style>