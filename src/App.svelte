<script>
    import Counter from "./Counter.svelte";
    export let name;
    export let initialCounter;

</script>

<main>
  <Counter name={name} initialCounter={initialCounter}/>
  <Counter name={name} initialCounter={initialCounter}/>
  <Counter name={name} initialCounter={initialCounter}/>
</main>