<div style="background-color: #{$hex};">
</div>

<script>
  import { getContext } from 'svelte'

  export let contextKey

  const { hex } = getContext(contextKey) 
</script>

<style>
	div {
		height: 100px;
		width: 100px;
	}
</style>