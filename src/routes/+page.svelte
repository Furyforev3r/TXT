<script lang="ts">
    import Logo from "$lib/images/logo.png"
    import GoogleIcon from "$lib/assets/google.svg"
</script>

<svelte:head>
    <title>TXT - Login</title>
</svelte:head>

<main>
    <section>
        <img class="logo" src={Logo} alt="Txt." />
        <div class="login">
            <div>
                <h1>Welcome to TXT.</h1>
                <p>Your favorite platform for smooth and efficient communication.</p>
            </div>
            <div class="divider"></div>
            <div>
                <button><img src={GoogleIcon} width="25px" alt="Google"> Login with Google!</button>
            </div>
        </div>
    </section>
</main>

<style>
    main {
        width: 100%;
        height: 100dvh;
        opacity: 1;
        background-image:  radial-gradient(#222 2px, transparent 2px), radial-gradient(var(--button-background) 2px, var(--background-color) 2px);
        background-size: 80px 80px;
        background-position: 0 0,40px 40px;
    }

    section {
        height: 100%;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
    }

    .logo {
        border-radius: 50%;
        cursor: pointer;
        width: 250px;
        height: 250px;
        transition: scale 0.3s;
    }

    .logo:hover {
        scale: 103%;
    }
    
    .login {
        background: var(--button-background);
        display: flex;
        flex-direction: column;
        gap: 0.4rem;
        padding: 1rem;
        border-radius: 0.8rem;
    }

    .divider {
        align-self: center;
        width: 95%;
        padding: 1px;
        border-radius: 0.3rem;
        background: var(--red-secondary-color);
    }

    button {
        width: 100%;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: center;
        gap: 0.4rem;
        cursor: pointer;
        background: none;
        padding: 1rem;
        border-radius: 999px;
        border: 0.2rem solid var(--focusBorder);
        color: var(--text-subdued);
        transition: 0.3s border-color;
        transition: 0.3s background;
    }

    button:hover {
        border-color: var(--foreground);
        background: var(--button-hover);
    }

    @media (max-width: 800px) {
        section {
            flex-direction: column;
            gap: 1rem;
        }
    }
</style>