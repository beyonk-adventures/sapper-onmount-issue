<div style="background-color: #{$currentColour};">
</div>

<script>
  import { readable } from 'svelte/store'

  export let hex

  const currentColour = readable(hex)
</script>

<style>
	div {
		height: 100px;
		width: 100px;
	}
</style>