<script>
    export let icon_left;
    export let icon_right;
    export let page_title;
    export let page_subtitle;
</script>

<div id="page_title" class="w-screen mt-4 pt-16 pb-16 text-center flex flex-col md:bg-no-repeat lg:bg-cover lg:bg-center lg:bg-[url('assets/header_img.png')] bg-[url('./assets/banner_background.png')]">
    <div class="flex justify-center">
        {@html icon_left}
        <h1 class="h1 font-bold px-4">{@html page_title}</h1>
        {@html icon_right}
    </div>
    <div class="flex justify-center py-4">
        <hr class="bg-primary-500 w-48 h-0.5">
    </div>
    <h4 class="h4 sm:mx-24 mx-2">{@html page_subtitle}</h4>
</div>

<style>
</style>