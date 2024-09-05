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

![GeoSimAI Interface](/assets/figs/geosimai_chat_interface_2.png)

## Demos

### General GeoSim.AI Demos

<div id="general-demos-carousel" class="video-carousel" style="max-width: 800px; margin: 0 auto; position: relative;">
  <div class="video-container" style="display: flex; justify-content: center; align-items: center;"></div>
  <div class="prev-video nav-arrow" style="left: -50px;">&lsaquo;</div>
  <div class="next-video nav-arrow" style="right: -50px;">&rsaquo;</div>
</div>

### ADONIS AI Agent Demos

<div id="adonis-demos-carousel" class="video-carousel" style="max-width: 800px; margin: 0 auto; position: relative;">
  <div class="video-container" style="display: flex; justify-content: center; align-items: center;"></div>
  <div class="prev-video nav-arrow" style="left: -50px;">&lsaquo;</div>
  <div class="next-video nav-arrow" style="right: -50px;">&rsaquo;</div>
</div>

### HYRCAN AI Agent Demos

<div id="hyracan-demos-carousel" class="video-carousel" style="max-width: 800px; margin: 0 auto; position: relative;">
  <div class="video-container" style="display: flex; justify-content: center; align-items: center;"></div>
  <div class="prev-video nav-arrow" style="left: -50px;">&lsaquo;</div>
  <div class="next-video nav-arrow" style="right: -50px;">&rsaquo;</div>
</div>

### AI Agents for Commercial Software

Demos related to agents for commerical software are for internal use only at the moment.

<style>
  .nav-arrow {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    cursor: pointer;
    font-size: 48px;
    color: #333;
    background-color: rgba(255, 255, 255, 0.7);
    width: 50px;
    height: 50px;
    border-radius: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const carousels = [
    {
      id: 'general-demos-carousel',
      videos: [
        { title: "Demo of GeoSim.AI Interface", id: "_LprVXHBT-I" }
      ]
    },
    {
      id: 'adonis-demos-carousel',
      videos: [
        { title: "ADONIS Demo 1", id: "Te3kfmKfaSA" }
      ]
    },
    {
      id: 'hyracan-demos-carousel',
      videos: [
        { title: "HYRCAN Demo 1", id: "NVIivwbvIMg" }        
      ]
    }
  ];

  carousels.forEach(carousel => {
    let currentVideoIndex = 0;
    const videoContainer = document.querySelector(`#${carousel.id} .video-container`);
    const prevArrow = document.querySelector(`#${carousel.id} .prev-video`);
    const nextArrow = document.querySelector(`#${carousel.id} .next-video`);

    function showVideo(index) {
      const video = carousel.videos[index];
      videoContainer.innerHTML = `
        <div>
          <h3 style="text-align: center;">${video.title}</h3>
          <iframe width="760" height="428" src="https://www.youtube.com/embed/${video.id}" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
      `;
    }

    prevArrow.addEventListener('click', function() {
      currentVideoIndex = (currentVideoIndex - 1 + carousel.videos.length) % carousel.videos.length;
      showVideo(currentVideoIndex);
    });

    nextArrow.addEventListener('click', function() {
      currentVideoIndex = (currentVideoIndex + 1) % carousel.videos.length;
      showVideo(currentVideoIndex);
    });

    showVideo(currentVideoIndex);
  });
});
</script>
