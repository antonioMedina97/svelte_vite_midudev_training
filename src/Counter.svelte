    <script>
        export let name;
        export let initialCounter;

        export let clicks = initialCounter ?? 0;

        function handleClick(){
            clicks++
        }
    </script>

    <div>
        <h1>Hello {name}, {clicks} times</h1>
    </div>
    <div>
        <button on:click={handleClick}>Counter</button>
    </div>