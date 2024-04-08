<font id="line1" color="#FF0000">  ██████╗ ██████╗ ███╗   ███╗██╗███╗   ██╗ ██████╗</font>
<font id="line2" color="#FF4500">  ██╔════╝██╔═══██╗████╗ ████║██║████╗  ██║██╔════╝</font>
<font id="line3" color="#FFFF00">  ██║     ██║   ██║██╔████╔██║██║██╔██╗ ██║██║  ███╗</font>
<font id="line4" color="#00FF00">  ██║     ██║   ██║██║╚██╔╝██║██║██║╚██╗██║██║   ██║</font>
<font id="line5" color="#1E90FF">  ╚██████╗╚██████╔╝██║ ╚═╝ ██║██║██║ ╚████║╚██████╔╝</font>
<font id="line6" color="#8A2BE2">   ╚═════╝ ╚═════╝ ╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝ ╚═════╝</font>

<script>
function animateColors() {
    let lines = document.querySelectorAll('font');
    lines.forEach((line, index) => {
        setInterval(() => {
            let randomColor = '#' + Math.floor(Math.random()*16777215).toString(16);
            line.setAttribute('color', randomColor);
        }, (index + 1) * 1000);
    });
}

animateColors();
</script>
