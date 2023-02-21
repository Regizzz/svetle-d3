<script>
    import { onMount } from "svelte";
    import * as d3 from "d3";

    onMount(() => {
        let myData = ["Hola Mundo!"];

        let p = d3.select(".hola")
              .data(myData)
              .text(function (d) {
                return d;
              })
    })
</script>

<p class="hola">another shitty text for ya</p>