<script>
    import { onMount } from "svelte";
    import * as d3 from "d3";

    onMount(() => {
        d3.select(".someshit")
          .on("mouseover", function() {
            d3.select(this)
              .style("background-color", "#4F46E5");

            // current event info
            console.log(d3.event);

            // x $ y coordinates info
            console.log(d3.mouse(this));
          })
          .on("mouseout", function() {
            d3.select(this)
              .style("background-color", "#9333EA")
          })
    })
</script>

<div class="someshit"></div>

<style>
    .someshit {
        height: 20vh;
        width: 20dvw;
        background-color: #9333EA;
        margin: 5px;
    }
</style>