<script>
    let mousePos = { x: 0, y: 0 };

    const handleMouseMove = (event) => {
        mousePos.x = event.clientX;
        mousePos.y = event.clientY;
    }
</script>

<style>
    div.mouse-pos {
        width: 70%;
        margin: 1em auto;
        padding: 1em;
        height: 10rem;
        background: #444;
        color: cornflowerblue;
        border: 2px solid cornflowerblue;
    }
</style>

<h3>Mouse over the box to calculate cursor position!</h3>
<div class="mouse-pos" on:mousemove={handleMouseMove}>
    Cursor Position is: {mousePos.x} &times; {mousePos.y}
</div>