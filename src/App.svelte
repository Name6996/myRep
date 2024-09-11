<script>
import Nested from './Nested.svelte';
</script>


<main>
<div class="container">

  <div class="element">
  Element 1
  </div>

  <div class="element">
  Element 2<Nested t2={count} /> 
  </div>

   <div class="element">
   Element 3
</div>

</div>
<Nested t2={test} />
</main>

<style>
.container {

  display: grid;

  grid-template-columns: 1fr auto 2fr;

  gap: 50px;

}


.element:first-child {

  grid-column: 1;

}


.element:last-child {

  grid-column: 3;

  justify-self: center;

}
</style>

<button on:click={increment}>
	цифры {count}
	{count === 1 ? 'time' : 'просто цифры'}
</button>
 





