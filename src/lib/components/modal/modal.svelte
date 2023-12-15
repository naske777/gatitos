<script>
    import { onMount } from "svelte";
    export let isOpen = false;
    import { fade } from 'svelte/transition';

    let modal
    onMount(() => {
        modal = new bootstrap.Modal(modal);
        console.log("ddd");
        if (isOpen) {
            modal.show();
            isOpen = false
         }
    });
</script>


<div bind:this={modal} class="modal rounded modal-lg" tabindex="-1" transition:fade={{ duration: 150 }}>
    <div class="modal-dialog">
        <div class="modal-content">
                <button type="button" class=" btn-close rounded-circle p-2 fs-6 position-absolute top-0 end-0 translate-middle-y bg-info" data-bs-dismiss="modal" aria-label="Close"></button>
            <div class="modal-body">
                <div class="row">
                    <!-- Primer elemento (4 columnas) -->
                    <div class="col-md-4 px-1">
                        <div class="content ">
                            <img src="/gatito2.jfif"  class="card-img-top rounded card-img " alt="gatito" />
                        </div>
                    </div>

                    <!-- Segundo elemento (5 columnas) -->
                    <div class="col-md-5 px-1">
                        <div class="content">
                            <img src="/gatito2.jfif"  class="card-img-top rounded card-img " alt="gatito" />
                        </div>
                    </div>

                    <!-- Tercer elemento (3 columnas) -->
                    <div class="col-md-3 px-1">
                        <div class="content">
                            <img src="/gatito2.jfif"  class="card-img-top rounded card-img-small " alt="gatito" />
                            <img src="/gatito2.jfif"  class="card-img-top rounded card-img-small " alt="gatito" />

                        </div>
                    </div>
                </div>

                <div class="row mt-4">
                    <div class="col-md-4">
                        <div class="content">
                            <h6 class="text-primary">¡Azul te lo cuenta!</h6>
                        </div>
                    </div>

                    <div class="col-md-8 mt-2">
                        <div class="content">
                            <div class="text-primary mb-4">
                            <h5>Papujo</h5>
                            <h6>El más viejo de las 4 colonias</h6>
                        </div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto reiciendis sint nobis sit voluptatem officia id ipsa nisi nostrum beatae expedita possimus eligendi laudantium dolores obcaecati temporibus, quis incidunt esse.</p>
                        </div>
                    </div>

                   
                </div>
               
            </div>
               
            <div class="d-flex justify-content-between px-4 py-2 bg-info align-items-center borderFixed">
                <h6 class="text-primary ">Ayuda a un gatito de la calle</h6>
                <button type="button" class="btn btn-warning  px-4 py-1 rounded-pill">Donar ahora</button>
         
            </div>
        </div>
        
    </div>
</div>

<style>
      .card-img {
        height: 200px;  /* Ajusta este valor según tus necesidades */
    }
    .card-img-small {
        height: 95px;  /* Ajusta este valor según tus necesidades */
    }
    img{
        margin-bottom: 10px
    }
    .borderFixed{
        border-radius: 0px 0px 6px 6px;
    }
</style>