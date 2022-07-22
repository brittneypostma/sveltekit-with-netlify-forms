<script context="module">
	export const prerender = true;
</script>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<form name="netlify-form-example" method="post" netlify netlify-honeypot="bot-field">
	<input type="hidden" name="netlify-form-example" value="netlify-form-example" />
	<input type="text" name="bot-field" />
	<p>
		<label>Your Name: <input type="text" name="name" /></label>
	</p>
	<p>
		<label>Your Email: <input type="email" name="email" /></label>
	</p>
	<p>
		<label>Message: <textarea name="message" /></label>
	</p>
	<p>
		<button type="submit">Send</button>
	</p>
</form>
