<script context="module">
	export const prerender = true;
</script>

<form name="netlify-form-example" method="POST" netlify-honeypot="bot-field" data-netlify="true">
	<input type="hidden" name="form-name" value="netlify-form-example" />
	<input name="name" required placeholder="Name" type="text" />
	<br />
	<input name="email" required placeholder="Email" type="email" />
	<br />
	<input name="message" required placeholder="Message" type="text" />
	<br />
	<input type="submit" value="Submit" />
</form>
