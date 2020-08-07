<Block {contextKey} />

<script>
  import { setContext } from 'svelte'
  import Block from './Block.svelte'
  import { readable } from 'svelte/store'

  const contextKey = {}

  export let hex

  $: hex && loadColour()

  function loadColour () {
    console.log('setting colour to', hex)
    setContext(contextKey, { hex: readable(hex) })
  }
</script>
