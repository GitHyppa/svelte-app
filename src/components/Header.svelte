<header>
	<h1>Janne.</h1>

	<nav>
		<a href="/">Home</a>
		<a href="/work">My work</a>
		<a href="/clients">Clients</a>
		<a href="/hire" id="hire">Hire me</a>
	</nav>

	<img id="menu" src="./menu.svg" alt="" />
</header>

<style>
	header {
		padding: 2.5rem 10%;
		display: flex;
		justify-content: space-between;
		align-items: center;
		margin-bottom: 10rem;
	}

	h1 {
		font-size: 1.5rem;
	}

	nav {
		display: none;
	}

	#menu {
		height: 25px;
	}

	@media (min-width: 1024px) {
		header {
			padding: 2.5rem 10%;
			display: flex;
			justify-content: space-between;
			align-items: center;
		}

		h1 {
			font-size: 2.5rem;
		}

		nav {
			display: flex;
			align-items: center;
			gap: 5rem;
			font-size: 1.25rem;
			font-weight: 300;
		}

		#menu {
			display: none;
		}

		#hire {
			padding: 0.5rem 1rem;
			background: #3f3fff;
			transition: 0.1s ease;
			font-weight: 500;
		}

		#hire:hover {
			background: #3030be;
		}
	}
</style>
