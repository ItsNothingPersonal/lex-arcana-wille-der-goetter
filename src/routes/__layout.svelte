<script>
	import '../app.css';
</script>

<nav class="bg-blue-900 shadow-lg">
	<a href="/">Home</a>
	<a href="/about">About</a>
	<a href="/settings">Settings</a>
</nav>

<div class="prose lg:prose-xl prose-headings:underline">
	<slot />
</div>
