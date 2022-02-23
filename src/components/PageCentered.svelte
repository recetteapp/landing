<div class="outer">
	<div class="inner">
		<slot />
	</div>
</div>

<style>
	.outer {
		display: flex;
		flex-flow: column nowrap;
		align-items: center;

		width: 100%;
		height: auto;
	}

	.inner {
		flex: 0 0 auto;

		width: min(350px, 100%);
		height: auto;
	}

	@media screen and (min-width: 600px) {
		.inner {
			width: 500px;
		}
	}

	@media screen and (min-width: 800px) {
		.inner {
			width: 700px;
		}
	}

	@media screen and (min-width: 1024px) {
		.inner {
			width: 900px;
		}
	}

	@media screen and (min-width: 1440px) {
		.inner {
			width: 1100px;
		}
	}
</style>
