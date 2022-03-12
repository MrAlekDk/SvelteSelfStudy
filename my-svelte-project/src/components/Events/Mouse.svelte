<script>

let location ={
    x:0,y:0
}

function mouseEvent(event){
    location.x = event.clientX;
    location.y = event.clientY;
}
</script>

<div on:mousemove={mouseEvent}>
The current position of the mouse is: x={location.x} y={location.y}
</div>

<div on:mousemove="{e => location = { x: e.clientX, y: e.clientY }}">
	The mouse position is {location.x} x {location.y}
    <br>This is made with inline even handler
</div>

<style>
	div { 
        width: 300px; 
        height: 300px; 
        border: solid 1px black;
        margin: 0 auto;
    }
</style>