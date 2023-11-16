<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Noto+Sans:wght@400;600;700&display=swap">
</head>

<script>
    export let icon;
    export let number;
    export let text;
    export let title;
</script>

<div class="m-2">
    <div id="cont" class="bg-surface-300 rounded-2xl">
        <div class="text-center p-4">
            <div class="flex justify-center pt-6">
                <div>{@html icon}</div>
            </div>
            <h3 class="h3 font-bold py-4">
                {title}
            </h3>
            <p class="text-center text-lg px-1">{text}</p>
        </div>
    </div>
    
    <div class="flex justify-center content-center">
        <div class="bg-primary-500 rounded-full -mt-8" id="num_cont">
            <h3 class="h3 pt-4 font-bold text-center">{number}</h3>
        </div>
    </div>
</div>

<style>
    #cont {
        height: 280px;
        width: 220px;
    }

    #num_cont {
        width: 4em;
        height: 4em;
    }

    h3, p {
        font-family: 'Noto Sans', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>
