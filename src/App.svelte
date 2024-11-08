<script>
  var x = 0
  import { onMount } from 'svelte';
  onMount(async () => {
    let data = await fetch('/api01.php').then(res => res.text());
    x = Number(data);
  })
</script>

<main>
  {x}
</main>

<style>
 
</style>
