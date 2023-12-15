<script>
	import Tips from "../tips/tips.svelte";

</script>

<div id="carouselExample" class="carousel carousel-dark slide">
    <div class="carousel-inner">
      <div class="carousel-item active">
        <Tips
        title={'Crueldad'}
        description={'Negarles aliemento, envenenarlos o abandonarlos son actos de crueldad'}
        body={'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum corporis, quisquam animi inventore labore ea laudantium sapiente molestiae aperiam architecto quas libero dolores, deserunt distinctio. Voluptas odio officiis facere hic.'}
      />      </div>
      <div class="carousel-item">
        <Tips
        title={'Crueldad'}
        description={'Negarles aliemento, envenenarlos o abandonarlos son actos de crueldad'}
        body={'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum corporis, quisquam animi inventore labore ea laudantium sapiente molestiae aperiam architecto quas libero dolores, deserunt distinctio. Voluptas odio officiis facere hic.'}
      />      </div>
      <div class="carousel-item">
        <Tips
        title={'Crueldad'}
        description={'Negarles aliemento, envenenarlos o abandonarlos son actos de crueldad'}
        body={'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nostrum corporis, quisquam animi inventore labore ea laudantium sapiente molestiae aperiam architecto quas libero dolores, deserunt distinctio. Voluptas odio officiis facere hic.'}
      />      </div>
    </div>
    <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>

  
