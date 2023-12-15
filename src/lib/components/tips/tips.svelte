<script>
export let title
export let description
export let body
</script>
<div class="d-flex flex-column align-items-center">
<div class="bg-white rounded card p-4 cardTips mb-4 align-items-center ">
<div class="row container">
    <div class="col-md-5 ">
        <div class="content text-primary ">
            <h4>{title}</h4>
            <br>
            <h6>{description}</h6>
        </div>
    </div>

    <div class="col-md-7 ">
        <div class="content ">
            <p class="text-primary">{body}</p>
        </div>
    </div>

</div>
</div>
</div>
<style>

    .cardTips{
        max-width: 600px;
        width: 100%;
    }
</style>