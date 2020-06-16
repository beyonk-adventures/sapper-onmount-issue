<script>
  const colours = {
    red: 'ff0000',
    blue: '0000ff',
    green: '00ff00'
  }
</script>

<ul>
  {#each Object.entries(colours) as [ colour, hex ]}
  <li>
    <a href="/colour/{hex}" rel="prefetch">See {colour}</a>
  </li>
  {/each}
</ul>