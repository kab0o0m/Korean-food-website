<head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&family=Noto+Sans:wght@400;600;700&display=swap">
</head>

<script>
    export let product_name;
    export let product;
    export let image_src;
</script>

<div class="flex flex-col px-6 py-2 select-none">
    <div class="pb-4 h-48 flex"><a href="{product}.html">
        <img src="{image_src}" alt=""
             class="hover:scale-110 hover:rotate-3 duration-150 -z-50"
        />
    </a></div>
    <h4 class="h4 py-2 hover:underline"><a href="{product}.html">{product_name}</a></h4>
</div>

<style>
    h4.h4 {
        font-family: 'Poppins', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>