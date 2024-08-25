---
layout: default
title: GeoSim.AI - Coming soon...
mathjax: true
---

### A new paradigm in computational geomechanics

The ability to accomplish tasks via natural language instructions is one of the most efficient forms of interaction between humans and technology. This efficiency has been translated into practical applications, with AI-powered chatbots and voice-activated virtual assistants now allowing users to interact through natural language queries. The emergence of advanced Large Language Models (LLMs) marks a pivotal shift in this direction. With ongoing advancements in the field of AI, integrating natural language commands into sophisticated technical fields in science and engineering is becoming increasingly feasible. This paper explores the transformative potential of LLMs in enhancing numerical simulations for computational geomechanics. We investigate how AI assistants powered by LLMs can streamline the process of creating complex simulation inputs and interpreting results by translating natural language instructions into precise technical commands and scripts. This approach aims to bridge the gap between human intent and the intricate requirements of numerical modeling tools, potentially revolutionizing how researchers and engineers interact with simulation software. We present a demonstrative application to illustrate this approach, discuss implementation challenges and benefits, and explore the future prospects of AI-assisted simulation workflows. Our findings highlight the potential of this technology to significantly enhance productivity and accessibility in computational geomechanics.

#### Architecture of GeoSim.AI

![GeoSimAI Architecture](/assets/figs/geosimai-architecture-v3.png)

#### GeoSim.AI Interface

![GeoSimAI Interface](/assets/figs/geosimai_chat_interface.png)

#### Demos

<div id="video-carousel" style="max-width: 660px; margin: 0 auto; position: relative;">
  <div id="video-container" style="display: flex; justify-content: center; align-items: center;"></div>
  <div id="prev-video" style="position: absolute; left: -30px; top: 50%; transform: translateY(-50%); cursor: pointer; font-size: 24px; color: #333;">&lt;</div>
  <div id="next-video" style="position: absolute; right: -30px; top: 50%; transform: translateY(-50%); cursor: pointer; font-size: 24px; color: #333;">&gt;</div>
</div>

**Demos coming soon...**

<script>
document.addEventListener('DOMContentLoaded', function() {
  const videos = [
    { title: "Example Chat", id: "U7zO1sHR3gQ" },
    { title: "Script Generation", id: "U7zO1sHR3gQ" }
  ];
  
  let currentVideoIndex = 0;
  const videoContainer = document.getElementById('video-container');
  const prevArrow = document.getElementById('prev-video');
  const nextArrow = document.getElementById('next-video');

  function showVideo(index) {
    const video = videos[index];
    videoContainer.innerHTML = `
      <div>
        <h3>${video.title}</h3>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/${video.id}" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
    `;
  }

  prevArrow.addEventListener('click', function() {
    currentVideoIndex = (currentVideoIndex - 1 + videos.length) % videos.length;
    showVideo(currentVideoIndex);
  });

  nextArrow.addEventListener('click', function() {
    currentVideoIndex = (currentVideoIndex + 1) % videos.length;
    showVideo(currentVideoIndex);
  });

  showVideo(currentVideoIndex);
});
</script>