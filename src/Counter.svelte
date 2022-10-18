    <script>

        export let initialCounter;

        export let clicks = initialCounter ?? 0;

        function handleClick(){
            clicks++
        }

        $: isEvenOrOdd = (clicks % 2 == 0) ? "even" : "odd"
    </script>


    <div>
        <h3>{clicks} is {isEvenOrOdd}</h3>
        <button on:click={handleClick}>Counter</button>
    </div>