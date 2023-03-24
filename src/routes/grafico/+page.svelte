<script>
    // Example from  https://svelte.dev/repl/8722c32f4e1a44a98e3a3fc8a095b2d7?version=3.5.3
    import { onMount } from "svelte";
    import * as d3 from "d3";
    var data = [30, 86, 168, 281, 303, 365];

    let el;

    onMount(() => {
        d3.select(el)
            .selectAll("div")
            .data(data)
            .enter()
            .append("div")
            .style("width", function (d) {
                return d + "px";
            })
            .text(function (d) {
                return d;
            });
    });
</script>

<div class="container">
    <br />
    <h1>Grafico de Barras</h1>

    <div id="grafico" />

    <p>
        Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation
    </p>

    <div bind:this={el} class="chart" />
</div>

<style>
    .chart :global(div) {
        font: 10px sans-serif;
        background-color: steelblue;
        text-align: right;
        padding: 3px;
        margin: 1px;
        color: white;
    }
</style>
