<script>
    import Card from '../card/cardGatitos.svelte';
    export let cards = [];
</script>

<div class="row row-cols-1 row-cols-md-3 g-4 ">
    {#each cards as card }
        <div class="col">
            <Card image={card.image} title={card.title} body={card.body} buscoH={card.buscoH} />
        </div>
    {/each}
</div>
