<script>
	import PageCentered from 'src/components/PageCentered.svelte';
	import Header from 'src/components/Header.svelte';

	let email = '';
	let password = '';
	let passwordConfirmation = '';
</script>

<Header />

<PageCentered>
	<h1>Sign Up</h1>

	<section class="form">
		<label for="email">Email</label>
		<input id="email" type="text" placeholder="johndoe@example.com" bind:value={email} />

		<label for="password">Password</label>
		<input id="password" type="password" placeholder="Choose something hard to guess" bind:value={password} />

		<label for="confirm-password">Confirm Password</label>
		<input id="confirm-password" type="password" placeholder="Now do it again" bind:value={passwordConfirmation} />

		<button>Create your account</button>

		<hr />

		<button>Sign up with Google</button>
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
