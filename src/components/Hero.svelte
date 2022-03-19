<section>
	<h1>Hello,<br />I'm <span>Janne!</span></h1>
	<p>Web Developer</p>

	<button>My work</button>

	<div id="scroll">
		<span class="active" />
		<span />
		<span />
	</div>
</section>

<style>
	h1 {
		font-size: 2.5rem;
		line-height: 100%;
	}

	span {
		color: #3f3fff;
	}

	p {
		font-size: 1.5rem;
		font-weight: 200;
		margin-top: 0.25rem;
	}

	button {
		padding: 1rem 2rem;
		margin-top: 2.5rem;
		background: #3f3fff;
		color: white;
		text-transform: uppercase;
		font-weight: 600;
		border-radius: 0.25rem;
	}

	button:hover {
		background: #3030be;
	}

	#scroll {
		position: absolute;
		right: 2.5rem;
		top: 50%;
		transform: translateY(-50%);
		display: flex;
		flex-direction: column;
		gap: 1rem;
	}

	#scroll > span {
		padding: 0.25rem;
		border-radius: 1rem;
		border: 1px solid #3f3fff;
	}

	#scroll > .active {
		background: #3f3fff;
	}

	@media (min-width: 1024px) {
		h1 {
			font-size: 4rem;
		}

		p {
			font-size: 2rem;
		}

		button {
			margin-top: 5rem;
			padding: 1.25rem 2.5rem;
			font-size: 1.25rem;
		}

		#scroll {
			right: 5rem;
		}

		#scroll > span {
			padding: 0.5rem;
		}
	}
</style>
