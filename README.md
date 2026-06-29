#TLE-PROJECT
<style>
body{
    background: #000;
    margin: 0;
    padding: 20px;
    overflow-y: auto;
    font-family: Arial, sans-serif;
}

#typing{
    font-size: 13px;     
    line-height: 1.6;
    color: white;
    max-width: 900px;
    margin: auto;
    white-space: pre-wrap;
}
</style>

<div id="typing"></div>

<script>
const text = `Hello and welcome to our website!

We are John Ernest S. Namora and Lhyod Emmanuel O. Mahor, Grade 10 students taking Technology and Livelihood Education (TLE) – Computer Systems Servicing (CSS).

This website was created to showcase our knowledge, skills, and projects developed throughout our CSS journey. It reflects our learning in computer hardware, software installation, troubleshooting, networking, and web development while allowing us to apply what we have learned in a meaningful way.

Our goal is to demonstrate our growth as students, highlight our creativity and technical skills, and inspire continuous learning in the field of technology. Every project we complete strengthens our problem-solving abilities and prepares us for future opportunities in the ever-evolving digital world.

Thank you for taking the time to visit our website. We hope you enjoy exploring our work and learning more about our journey in Computer Systems Servicing.`;

const typing = document.getElementById("typing");
let i = 0;

function type() {
    if (i < text.length) {
        typing.innerHTML += text.charAt(i) === "\n" ? "<br>" : text.charAt(i);
        i++;

        // Auto scroll while typing
        window.scrollTo({
            top: document.body.scrollHeight,
            behavior: "smooth"
        });

        setTimeout(type, 18);
    }
}

type();
</script>

