<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Noto+Sans:wght@400;600;700&display=swap">
</head>

<script>
    export let question = "Type your question!";
    export let answer = "Type your answer!";
    let isAnswerOpen = false;

    const toggleAnswer = () => {
        isAnswerOpen = !isAnswerOpen;
    }
</script>

<div class="flex py-4">
    <div class="px-4 pt-2">
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <!-- svelte-ignore a11y-no-static-element-interactions -->
        <svg on:click={toggleAnswer}
        class="{ isAnswerOpen ? 'rotate-90' : '' } transition-transform transform hover:rotate-90 " 
        xmlns="http://www.w3.org/2000/svg" height="1.25em" viewBox="0 0 512 512"><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path d="M0 256a256 256 0 1 0 512 0A256 256 0 1 0 0 256zM241 377c-9.4 9.4-24.6 9.4-33.9 0s-9.4-24.6 0-33.9l87-87-87-87c-9.4-9.4-9.4-24.6 0-33.9s24.6-9.4 33.9 0L345 239c9.4 9.4 9.4 24.6 0 33.9L241 377z"/></svg>
    </div>
    <div>
        <!-- svelte-ignore a11y-click-events-have-key-events -->
        <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
        <h3 class="h3 font-bold pb-2 hover:underline cursor-pointer" on:click={toggleAnswer}>{question}</h3>
        {#if isAnswerOpen}
            <p class="pr-8 text-justify">{@html answer}</p>
        {/if}
    </div>
</div>

<style>
    p, h3 {
        font-family: 'Noto Sans', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>