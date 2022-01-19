<form method="get" action="/search">
	<input type="search" name="q" id="search-input" placeholder="Search..." required />
  <button type="submit" id="search-submit" aria-label="Submit search">
	<svg
		class="w-6 h-6"
		data-darkreader-inline-stroke=""
		fill="none"
		stroke="currentColor"
		style="--darkreader-inline-stroke: currentColor;"
		viewBox="0 0 24 24"
		xmlns="http://www.w3.org/2000/svg"
		><path
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-width="2"
			d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"
		/></svg>
  </button>
</form>

<style lang="scss">
  form {
    display: flex;
    height: inherit;
    width: 20rem;
					 
		input {
			flex: 1;
		}
		
		button {
			aspect-ratio: 1;
		}
  }
</style>
