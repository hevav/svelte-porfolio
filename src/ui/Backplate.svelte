<script>
    export let color;
</script>

<div class="backplate" style="background-color: {color}">

</div>

<style>
    .backplate {
        transform: rotate(-3deg) skew(-3deg);
        width: 100vw;
        left: -2px;
        position: absolute;
        /*
            max-height: 420px;
            height: 40%;
        */
        height: 420px;
        top: -75px;
    }
</style>