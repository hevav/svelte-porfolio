<script>
    export let icon, text;
</script>

<div class="line">
    <i class={icon}></i>
    <span class="text">
        {text}
    </span>
</div>

<style>
    i {
        text-align: center;
        font-size: 1rem;
        width: 25px;
    }

    .line {
        margin: 0.5rem;
    }

    .text {
        font-size: 1.15rem;
        font-weight: bold;
        margin-left: 0.5rem;
    }
</style>