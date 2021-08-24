<script>
    export let header, logo, color;
    if (header) header = "url(" + header + ")";
    if (logo) logo = "url(" + logo + ")";
</script>

<div class="bound" style="background-color: {color}">
    {#if header !== undefined}
        <div class="header" style="background-image: {header}">
            {#if logo !== undefined}
                <div class="logo" style="border-color: {color}; background-image: {logo}"></div>
            {/if}
        </div>
    {/if}
    <div class="content">
        <slot></slot>
    </div>
</div>

<style>
    .bound {
        border-radius: 1rem;
        width: 100%;
        box-shadow: 0 0.25rem 0.5rem 0 rgba(0,0,0,.1);
    }

    .header {
        border-top-left-radius: 1rem;
        border-top-right-radius: 1rem;
        width: 100%;
        background-size: cover;
        background-position: center;
        height: 260px;
        position: relative;
        margin-bottom: 3.5rem;
    }

    .logo {
        border-radius: 100%;
        position: absolute;
        bottom: -5rem;
        left: 1rem;
        box-shadow: 0 2px 4px 0 rgba(0,0,0,.1);
        border: 1rem solid;
        width: 10rem;
        height: 10rem;
        background-size: contain;
    }

    .content {
        height: 100%;
    }


    @media (max-width: 720px) {
        .header {
            height: 120px;
        }

        .logo {
            width: 5rem;
            height: 5rem;
        }
    }
</style>