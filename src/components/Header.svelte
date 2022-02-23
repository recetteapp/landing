<script>
	import PageCentered from './PageCentered.svelte';
</script>

<header class="header-wrapper">
	<PageCentered>
		<div class="header">
			<h1 class="brand"><a href="/">Recette</a></h1>
			<div class="auth-links">
				<a class="auth-link" href="/signup">Sign Up</a>
				<a class="auth-link" href="/login">Log In</a>
			</div>
		</div>
	</PageCentered>
</header>

<style>
	.header-wrapper {
		background: lightblue;
		padding-top: 10px;
		padding-bottom: 10px;
	}
	.header {
		display: flex;
		flex-flow: row nowrap;
		align-items: center;
		justify-content: space-between;
	}

	.brand {
		margin: 0;
	}

	.auth-link {
		padding: 5px 7px;
		border: solid 2px black;
		border-radius: 5px;
	}
</style>
