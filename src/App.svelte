<script>
    import Counter from "./Counter.svelte";
    import Hello from "./Hello.svelte";
    export let name;
    export let initialCounter;

    let commonProps = { initialCounter }

</script>

<main>
  <Hello name={name} />
  <Counter { ... commonProps}/>
  <Counter initialCounter={5}/>
  <Counter initialCounter={initialCounter}/>
</main>