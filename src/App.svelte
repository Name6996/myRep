<script>
let name = 'DAAAA';
import Nested from './Nested.svelte';
</script>

<main>
<p>Hello world {name}</p>
<Nested />
</main>

<style>
p {color : green;
font-family: 'Comic Sans MS', cursive;
font-size: 2em; 
}
main {
		color: blue;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>


