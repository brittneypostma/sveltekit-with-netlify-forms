<script context="module">
	export const prerender = true;
</script>

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

<form name="netlify-form-example" method="POST" netlify-honeypot="bot-field" data-netlify="true">
	<input type="hidden" name="form-name" value="netlify-form-example" />
	<input name="name" required placeholder="Name" type="name" />
	<br />
	<input name="email" required placeholder="Email" type="email" />
	<br />
	<input name="message" required placeholder="Message" type="text" />
	<br />
	<input type="submit" value="Submit" />
</form>
