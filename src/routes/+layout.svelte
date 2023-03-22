<script>
    import Contacts from '$lib/Contacts.svelte';
	const favicon = "https://raw.githubusercontent.com/Maruf-co/Portfolio/main/src/content/favicon.ico";
	import {base} from '$app/paths';
	import './app.css';
</script>

<div class="app">
	<head>
		<!-- favicon -->
		<link type="image/x-icon" href={favicon} rel="shortcut icon">
		<link type="Image/x-icon" href={favicon} rel="icon">
		<!-- pixel fonts -->
		<link rel="preconnect" href="https://fonts.googleapis.com">
		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin=true >
		<link
		  href="https://fonts.googleapis.com/css2?family=Silkscreen&display=swap"
		  rel="stylesheet"
		>
		<meta name="viewport" content="width=device-width" />
		<title>Anna's portfolio</title>
	</head>
	<header>
		<nav>
			<div class="container">
			  <a class="navItem author" href="{base}/"><b>Relisqu</b></a>
			  <a class="navItem" href="{base}/projects">Projects</a>
			  <a class="navItem" href="{base}/jokes">Jokes</a>
			</div>
		</nav>
	</header>

	<main>
		<slot />
	</main>

	<footer>
		<Contacts />
	</footer>
</div>
