<script lang="ts">
    import Logo from "$lib/images/logo.png"
</script>

<svelte:head>
    <title>TXT - Welcome!</title>
</svelte:head>

<main>
    <img src={Logo} alt="Txt." />

    <div class="description">
        <div>
            <h1>Welcome to TXT.</h1>
            <p>Your favorite platform for smooth and efficient communication.</p>
        </div>
        <button>Get Started</button>
    </div>
</main>

<style>
    main {
        height: 100dvh;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
    }

    img {
        border-radius: 50%;
        cursor: pointer;
        width: 250px;
        height: 250px;
        transition: scale 0.3s;
    }

    img:hover {
        scale: 103%;
    }

    div {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .description {
        border-radius: 0.8rem;
        gap: 0.8rem;
    }

    .description button {
        align-self: center;
        display: flex;
        align-items: center;
        cursor: pointer;
        color: var(--text-alternative);
        padding: 1.2rem;
        background: var(--blue-primary-color);
        border: none;
        border-radius: 0.8rem;
        transition: 0.3s background;
    }

    .description button:hover {
        background: var(--blue-secondary-color);
    }
</style>