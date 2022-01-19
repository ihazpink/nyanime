<script context="module" lang="ts">
	//** @type {import('@sveltejs/kit').Load} */
	export async function load({ url }) {
		const query: string = url.searchParams.get('q');

		// If there is no query we return to index
		if (!query) {
			return {
				status: 302,
				redirect: '/'
			};
		}

		return {};
	}
</script>

<script lang="ts">
	import { page } from '$app/stores';
	const query = $page.url.searchParams.get('q');
</script>

<h1>{query}</h1>
