<script>
    import { onMount } from "svelte";
    import * as d3 from "d3";

    onMount(() => {
        d3.select("#container")
          .transition()
          .duration(2000)
          .style("background-color", "#DB2777")
    })
</script>

<div id="container">

</div>

<style>
    #container {
        height: 20vh;
        width: 20vw;
        background-color: #7C3AED;
    }
</style>