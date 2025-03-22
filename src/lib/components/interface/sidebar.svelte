<script lang="ts">
    import Logo from "$lib/images/logo.png"
    import Icon from "@iconify/svelte"
</script>

<div class="sidebar">
    <ul>
        <div class="icons">
            <li>
                <a href="/" class="icon">
                    <Icon icon="bx:bx-home" width="28px" height="28px" color="#888" />
                </a>
            </li>
            <li>
                <a href="/" class="icon">
                    <Icon icon="bx:bx-message-square-detail"  width="28px" height="28px" color="#888" />
                </a>
            </li>
            <li>
                <a href="/" class="icon">
                    <Icon icon="bx:bx-group"  width="28px" height="28px" color="#888" />
                </a>
            </li>
        </div>
        <div class="icons">
            <li>
                <a href="/" class="icon">
                    <Icon icon="bx:bx-cog"  width="28px" height="28px" color="#888" />
                </a>
            </li>
            <li>
                <a href="/" class="profile">
                    <img src={Logo} alt="Placeholder." class="profileImage" width="46px"/>
                </a>
            </li>
        </div>
    </ul>
</div>

<style>
    .sidebar {
        background-color: var(--sideBar-background);
        width: 50px;
        padding: 1rem;
        border-right: solid 1px var(--blue-primary-color);
        height: 100%;
        max-height: 100%;
    }
    
    .sidebar, .sidebar ul {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .sidebar ul {
        height: 100%;
        justify-content: space-around;
    }

    .icons {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1.2rem;
    }

    .icon {
        display: grid;
        place-items: center;
        padding: 1rem;
        cursor: pointer;
        border-radius: 0.8rem;
        transition: background-color 0.3s;
    }

    .icon:hover {
        background-color: var(--blue-primary-color);
    }

    .profile {
        display: grid;
        place-items: center;
        cursor: pointer;
    }

    .profileImage {
        border-radius: 50%;
    }
</style>
