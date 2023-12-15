<script>
	import CardGatitosContainer from '$lib/components/cardContainer/cardGatitosContainer.svelte';
	import Carousel from '../lib/components/carousel/carousel.svelte';
	import Pagination from '../lib/components/pagination/pagination.svelte';
	import Tips from '../lib/components/tips/tips.svelte';

	let cards = [
		{
			buscoH: true,
			image: '/gatito.jfif',
			title: 'Título 1',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			image: '/gatito.jfif',
			title: 'Título 2',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			buscoH: true,
			image: '/gatito.jfif',
			title: 'Título 3',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			image: '/gatito.jfif',
			title: 'Título 4',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			buscoH: true,
			image: '/gatito.jfif',
			title: 'Título 5',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			image: '/gatito.jfif',
			title: 'Título 6',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			image: '/gatito.jfif',
			title: 'Título 7',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			buscoH: true,
			image: '/gatito.jfif',
			title: 'Título 8',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		},
		{
			buscoH: true,
			image: '/gatito.jfif',
			title: 'Título 9',
			body: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec viverra nec nulla vitae mollis'
		}
	];
</script>

<h4 class="mb-4 text-primary">Los gatitos de la EQUS</h4>
<CardGatitosContainer {cards} />

<Pagination/>
<h5 class="text-primary text-center mb-4 ">Peligros de una vida callejera</h5>

<Carousel/>