<script>
	import { menu } from '$lib/utils/menu';
	import { addToBag } from '$lib/utils/store.js';
</script>

{#each menu as item}
	<div class="card w-96 bg-base-100 shadow-xl">
		<div class="card-body items-center text-center">
			<h2 class="card-title">{item.nombre}</h2>
			<p>${item.precio}</p>
			<div class="card-actions">
				<button class="btn btn-primary" on:click={addToBag(item)}>Add to bag</button>
			</div>
		</div>
	</div>
{/each}
