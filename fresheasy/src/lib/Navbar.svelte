<script>
    import { Link } from 'svelte-routing';
</script>


<div id="main-header">
    <nav>
        <ul>
            <li><Link to="/">Home</Link></li>
            <li><Link to="/about">About</Link></li>
            <li><Link to="/posts">Posts</Link></li>
        </ul>
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
