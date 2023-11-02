<script>
    let count = 1;

    const increment = () => {  count += 1;  }
    const decrement = () => {  
        if (count > 0) {
            count -= 1;
        }
    }
</script>

<div class="flex w-24 h-9 select-none border-solid border-2 border-gray-300">
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <div class="w-8 flex pb-1 justify-center content-center text-xl hover:font-black hover:cursor-pointer" on:click={decrement}>-</div>
    <div class="w-8 flex pb-1 justify-center content-center font-bold pt-1">{count}</div>
    <!-- svelte-ignore a11y-no-static-element-interactions -->
    <!-- svelte-ignore a11y-click-events-have-key-events -->
    <div class="w-8 flex pb-1 justify-center content-center text-xl hover:font-black hover:cursor-pointer" on:click={increment}>+</div>
</div>