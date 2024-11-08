<script>
  var x
  import { onMount } from 'svelte';
  onMount(async () => {
    let data = await fetch('/api01.php').then(res => res.text());
    x = data;
  })
</script>

<main>
  {x}
</main>

<style>
 
</style>
