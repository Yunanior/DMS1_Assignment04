---
title: Week 10
published_at: 2024-05-27
snippet: Reflection writing
disable_html_sanitization: true
allow_math: true
---

# Reflection writing

**Assignment 01**

In reflecting on the project, the integration of sonic and visual elements was pivotal. The ambient sounds, such as heartbeats and equipment beeping, were meticulously synchronized with visual transitions, crafting a cohesive and emotionally resonant experience. This approach ensured that the auditory elements enhanced the narrative, making the themes of life and death more poignant and immersive. The footage selection process was equally deliberate, aiming to effectively convey the emotional journey. Symbolic elements like the dragonfly were chosen for their visual impact and thematic relevance, with iterative refinements ensuring alignment with the project's narrative and aesthetic goals.

The project underscored the power of sound in shaping emotional experiences. Background music and ambient sounds were chosen to evoke feelings of nostalgia and introspection. Techniques like L and J cuts facilitated seamless audio-visual transitions, heightening the viewer's emotional engagement. Through this project, the intricate interplay between sound and visual components was explored, demonstrating how carefully curated audio elements can amplify the emotional depth of visual storytelling.

**Assignmnet02**

The suite of icons was conceived with the theme of "Memory" in mind, targeting users passionate about documenting their lives. This theme was selected to resonate with individuals who keep diaries or film family moments, aiming to evoke a sense of nostalgia and personal history. The design process involved multiple iterations, starting with thumbnail sketches and evolving through feedback and refinement. Each iteration aimed to improve clarity and visual appeal, ensuring the final icons were functional and aesthetically pleasing.

Color played a crucial role in creating a unified and visually appealing icon set. A palette of light blue, red, and yellow was chosen for its vibrancy and ability to convey the theme of memory. This color scheme added depth and made the icons more engaging, enhancing the user experience. The project highlighted the importance of iterative design and the thoughtful use of color to create a cohesive and meaningful user interface.


**Assignment03**

Creating a working prototype was essential for identifying and resolving practical issues that theoretical planning could not foresee. It allowed for iterative testing and adjustments, such as fixing navigation problems and collider meshes, ensuring a smoother user experience. This hands-on approach was instrumental in refining the design and functionality of the project.

Designing a 3D environment required different considerations compared to 2D media. The 3D project demanded a focus on spatial awareness, depth, and user interaction, whereas 2D design primarily dealt with layout and visual balance. This shift in focus was both challenging and enriching, offering a broader perspective on design principles. The virtual camera played a pivotal role in guiding the user's perspective and enhancing immersion. Unlike in previous assignments where the camera captured specific angles, the virtual camera in the 3D environment allowed for dynamic exploration, providing a more interactive and engaging experience.

Sound was used to create atmosphere and emotional depth, similar to previous assignments but adapted for a 3D environment. Background music was chosen to evoke a sense of order and immersion, while ambient sounds like birds singing were used sparingly to maintain a peaceful atmosphere. This approach differed from earlier projects where sound was more directly tied to visual transitions. The theme of "Life and Death" guided the design, evolving from initial sketches to a more refined concept that balanced fantasy and realism. Play testing uncovered issues that were not apparent during the design phase, such as navigation problems and model collisions, highlighting the importance of user feedback in the iterative design process.



## Statement Writing




## Maths:

... which can be written inline, like this: $\{ x, y, z \} \in \N$

... or block, like this:

$$ x^2 + y^2 = z^2 $$

Visit [ $\KaTeX$ ](https://katex.org/docs/supported#fractions-and-binomials) for more information about writing maths.

## Embedding video:

<iframe id="coding_train_video" src="https://www.youtube.com/embed/rI_y2GAlQFM?si=RDgjkpunxk1mQzMI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<script type="module">

    console.log (`hello world! 🚀`)

    const iframe  = document.getElementById (`coding_train_video`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16

</script>

## Embedding p5 sketches:

<iframe id="falling_falling" src="https://editor.p5js.org/capogreco/full/Fkg05m7aA"></iframe>

<script type="module">

    const iframe  = document.getElementById (`falling_falling`)
    iframe.width  = iframe.parentNode.scrollWidth
    iframe.height = iframe.width * 9 / 16 + 42

</script>

## Canvas API

<canvas id="canvas_example"></canvas>

<script type="module">
    const cnv = document.getElementById (`canvas_example`)
    cnv.width = cnv.parentNode.scrollWidth
    cnv.height = cnv.width * 9 / 16

    const ctx = cnv.getContext (`2d`)
    const pos = {
        x: -100,
        y: cnv.height / 2 - 50
    }
    
    function draw_frame () {
        ctx.fillStyle = `turquoise`
        ctx.fillRect (0, 0, cnv.width, cnv.height)

        ctx.fillStyle = `hotpink`
        ctx.fillRect (pos.x, pos.y, 100, 100)

        pos.x += 2

        if (pos.x > cnv.width) {
            pos.x = -100
        }

        requestAnimationFrame (draw_frame)
    }

    draw_frame ()
</script>


