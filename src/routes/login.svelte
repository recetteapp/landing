<script>
	import PageCentered from 'src/components/PageCentered.svelte';
	import Header from 'src/components/Header.svelte';

	let email = '';
	let password = '';
</script>

<Header />

<PageCentered>
	<h1>Log In</h1>

	<section class="form">
		<label for="email">Email</label>
		<input id="email" type="text" placeholder="johndoe@example.com" bind:value={email} />

		<label for="password">Password</label>
		<input id="password" type="password" placeholder="You should know this" bind:value={password} />

		<button>Log in</button>

		<hr />

		<button>Log in with Google</button>
	</section>
</PageCentered>

<style>
	.form {
		display: flex;
		flex-flow: column nowrap;
		width: min(350px, 100%);

		padding: 24px;
		border: solid 1px black;
		border-radius: 7px;
	}

	.form hr {
		width: 100%;
	}
</style>
