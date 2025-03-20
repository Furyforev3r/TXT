<script lang="ts">
    import Logo from "$lib/images/logo.png"
</script>

<svelte:head>
    <title>TXT - Welcome!</title>
</svelte:head>

<main>
    <img src={Logo} alt="Txt." />
</main>

<style>
    main {
        display: grid;
        place-items: center;
        height: 100vh;
    }

    img {
        border-radius: 50%;
        cursor: pointer;
        width: 250px;
        height: 250px;
        transition: box-shadow 0.3s;
    }

    img:hover {
        -webkit-box-shadow: 0px 0px 20px 0px var(--button-background);
        -moz-box-shadow: 0px 0px 20px 0px var(--button-background);
        box-shadow: 0px 0px 20px 0px var(--button-background);
    }
</style>