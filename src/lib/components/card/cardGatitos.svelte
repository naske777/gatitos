<script>
	import Modal from "../modal/modal.svelte";

    export let image;
    export let title;
    export let body;
    export let buscoH;
    let isOpen
    function openModal() {
        isOpen = false
        setTimeout(() => {
            isOpen = true
        }, 10);
       
    }
</script>

<!-- svelte-ignore a11y-click-events-have-key-events -->
<!-- svelte-ignore a11y-no-static-element-interactions -->
<div class="card m-4 bg-white rounded cursor-pointer" on:click={openModal}>
    <img src={image}  class="card-img-top rounded card-img " alt={title} />
    <div class="card-body">
        <div class="p-3 pt-0">
                   <div class="d-flex">
        <h5 class="card-title">{title}</h5>
        {#if buscoH}
        <h6 class="bg-success rounded-circle p-3 fs-6 position-absolute top-0 end-0 translate-middle-y text-white">Busco <br> Hogar</h6>

        {/if}
    </div>

        <p class="card-text">{body}</p>
        <a href="#" class="btn btn-info border-0 rounded-pill">Saber más</a>
    </div>
</div>
</div>
{#key isOpen}
    <Modal {isOpen}/>
{/key}
<style>
    .card-img {
        height: 300px;  /* Ajusta este valor según tus necesidades */
    }
    .cursor-pointer{
        cursor: pointer;
    }
</style>