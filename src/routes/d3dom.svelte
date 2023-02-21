<script>
    import { onMount } from "svelte";
    import * as d3 from "d3";

    // some data
    var data = [100, 200, 300];
    onMount(() => {
        
        // DOM selection
        var paragraph = d3.select("body")
                .selectAll("p")
                .data(data)
                .text(function (d, i) {
                    console.log("d: " + d);
                    console.log("i: " + i);
                    console.log("this: " + this);

                    return d;
                })
    })

</script>


<p></p>

<p></p>

<p></p>

