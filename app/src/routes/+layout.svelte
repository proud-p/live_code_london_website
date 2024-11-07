<script>
	import '../app.css';
	let { children } = $props();
</script>

<!-- <nav>
	<a href="/">Home</a>
	<a href="/about">About</a>
	<a href="/resources">Resources</a>
	<a href="/events">Events</a>
	<a href="/donate">Donate</a>
	<a href="/faq">FAQ</a>
  </nav> -->

{@render children()}
