<script>
    import Contacts from '../lib/Contacts.svelte';
	import Navbar from '../lib/Navbar.svelte'
	import './app.css';
</script>


<div class="app">
	<head>
		<!-- favicon -->
		<link type="image/x-icon" href="/favicon.ico" rel="shortcut icon">
		<link type="Image/x-icon" href="/favicon.ico" rel="icon">
		<!-- pixel fonts -->
		<link rel="preconnect" href="https://fonts.googleapis.com">
		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
		<link
		  href="https://fonts.googleapis.com/css2?family=Silkscreen&display=swap"
		  rel="stylesheet"
		>
		<meta name="viewport" content="width=device-width" />
		<title>Anna's portfolio</title>
	</head>
	<header>
		<Navbar />
	</header>

	<main>
		<slot />
	</main>

	<footer>
		<Contacts />
	</footer>
</div>
