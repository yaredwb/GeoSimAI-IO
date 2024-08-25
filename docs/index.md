<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GeoSim.AI - Coming soon...</title>
    <style>
        .video-carousel {
            position: relative;
            max-width: 560px;
            margin: 0 auto;
        }
        .video-container {
            display: none;
        }
        .video-container.active {
            display: block;
        }
        .nav-arrow {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            background-color: rgba(0,0,0,0.5);
            color: white;
            padding: 10px;
            text-decoration: none;
            font-size: 18px;
        }
        .nav-arrow.left {
            left: 10px;
        }
        .nav-arrow.right {
            right: 10px;
        }
    </style>
</head>
<body>
    <h1>GeoSim.AI - Coming soon...</h1>

    <h2>A new paradigm in computational geomechanics</h2>

    <p>The ability to accomplish tasks via natural language instructions is one of the most efficient forms of interaction between humans and technology. This efficiency has been translated into practical applications, with AI-powered chatbots and voice-activated virtual assistants now allowing users to interact through natural language queries. The emergence of advanced Large Language Models (LLMs) marks a pivotal shift in this direction. With ongoing advancements in the field of AI, integrating natural language commands into sophisticated technical fields in science and engineering is becoming increasingly feasible. This paper explores the transformative potential of LLMs in enhancing numerical simulations for computational geomechanics. We investigate how AI assistants powered by LLMs can streamline the process of creating complex simulation inputs and interpreting results by translating natural language instructions into precise technical commands and scripts. This approach aims to bridge the gap between human intent and the intricate requirements of numerical modeling tools, potentially revolutionizing how researchers and engineers interact with simulation software. We present a demonstrative application to illustrate this approach, discuss implementation challenges and benefits, and explore the future prospects of AI-assisted simulation workflows. Our findings highlight the potential of this technology to significantly enhance productivity and accessibility in computational geomechanics.</p>

    <h3>Architecture of GeoSim.AI</h3>
    <img src="/assets/figs/geosimai-architecture-v3.png" alt="GeoSimAI Architecture">

    <h3>GeoSim.AI Interface</h3>
    <img src="/assets/figs/geosimai_chat_interface.png" alt="GeoSimAI Interface">

    <h3>Demos</h3>
    <div class="video-carousel">
        <div class="video-container active">
            <h4>Example Chat</h4>
            <iframe width="560" height="315" src="https://www.youtube.com/embed/U7zO1sHR3gQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
        <div class="video-container">
            <h4>Script Generation</h4>
            <iframe width="560" height="315" src="https://www.youtube.com/embed/U7zO1sHR3gQ" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
        </div>
        <a href="#" class="nav-arrow left">&lt;</a>
        <a href="#" class="nav-arrow right">&gt;</a>
    </div>

    <p><strong>Demos coming soon...</strong></p>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const containers = document.querySelectorAll('.video-container');
            const leftArrow = document.querySelector('.nav-arrow.left');
            const rightArrow = document.querySelector('.nav-arrow.right');
            let currentIndex = 0;

            function showVideo(index) {
                containers.forEach((container, i) => {
                    if (i === index) {
                        container.classList.add('active');
                    } else {
                        container.classList.remove('active');
                    }
                });
            }

            leftArrow.addEventListener('click', function(e) {
                e.preventDefault();
                currentIndex = (currentIndex - 1 + containers.length) % containers.length;
                showVideo(currentIndex);
            });

            rightArrow.addEventListener('click', function(e) {
                e.preventDefault();
                currentIndex = (currentIndex + 1) % containers.length;
                showVideo(currentIndex);
            });
        });
    </script>
</body>
</html>