<script>
	import '../app.css';
	import Navbar from '../lib/components/Navbar.svelte';
	export let data;
</script>

<Navbar image={data.image} />
<slot />
