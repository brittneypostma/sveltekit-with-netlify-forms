<!-- <script context="module">
	export const prerender = true;
</script> -->

<!-- <script lang="ts">
	let isSubmitting: boolean = false;

	const handleSubmit = (e: Event) => {
		const form: HTMLFormElement | null = document.querySelector('form');
		const formData: FormData = new FormData(e.target as HTMLFormElement);
		let stringData: string = formData.toString();
		isSubmitting = true;
		return fetch('/', {
			method: 'POST',
			headers: { 'Content-Type': 'application/x-www-form-urlencoded' },
			body: new URLSearchParams(stringData)
		})
			.then(() => {
				console.log('Form successfully submitted');
				isSubmitting = false;
				form?.reset();
			})
			.catch((error) => {
				alert(error);
				isSubmitting = false;
			});
	};
</script> -->

<form name="netlify-form-example" method="post" netlify netlify-honeypot="bot-field">
	<input type="text" name="bot-field" hidden />
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
