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