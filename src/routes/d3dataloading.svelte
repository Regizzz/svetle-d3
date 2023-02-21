<script>
    import { csv } from "d3-fetch";
    import { onMount } from "svelte";
    import * as d3 from "d3";

    //var margin =  {top: 10, right: 30, bottom: 30, left: 60},
    //    width = 460 - margin.left - margin.right,
    //    height = 400 - margin.top - margin.bottom;
    
    //var svg = d3.select("#data_viz")
    //            .append("svg")
    //            .attr("width", width + margin.left + margin.right)
    //            .attr("height", height + margin.top + margin.bottom)
    //            .append("g")
    //            .attr("transform", "translate(" + margin.left + "," + margin.top + ")");

    onMount(() => {
        async function loadData() {
            return data = Object.assign(await csv('src/routes/strain-data-new.csv'))
        }
        loadData()
    })
</script>

<div id="data_viz"></div>