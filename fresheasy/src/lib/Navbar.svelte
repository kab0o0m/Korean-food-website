<script>
    import { Link } from 'svelte-routing';
</script>


<div id="main-header">
    <nav>
        <Link to="/">Home</Link>
        <Link to="/about">About</Link>
        <Link to="/posts">Posts</Link>
    </nav>
</div>


<style lang="scss">
    @import './../scss/colors.scss';
    #main-header {
        background-color: $background-primary;
        width: 100vw;
        margin-top:0px;
    }
</style>
