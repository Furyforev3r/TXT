<script>
	import '../app.css'
</script>

<div class="app">
	<slot />
</div>

<style>
	.app {
        overflow: hidden;
        width: 100%;
        height: 100dvh;
        display: flex;
        flex-direction: row;
	}
</style>