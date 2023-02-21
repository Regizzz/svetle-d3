<script>
    import D3shit from './d3dom.svelte'
    import D3events from './d3events.svelte'
    import D3animation from './d3animation.svelte';
    import D3databinding from './d3databinding.svelte';
    import D3dataloading from './d3dataloading.svelte';
</script>

<div class="flex flex-col border-2 border-indigo-700 bg-gray-200 min-h-screen justify-center items-center">
    <h1 class="text-xl">Hola Mundo!</h1>
    <div class="data border-4 border-dotted border-indigo-500">
        <!-- 
        <D3shit />
        <D3events />
        <D3animation />
        <D3databinding />
        -->
        <D3dataloading />
    </div>
    
</div>

<style>
    .data {
        margin: 1rem;
        height: 50vh;
        width: 50vw;
    }
</style>