<script>
  /* export let title; */
  export let links;
  export let links2;
  export let links3;
</script>

<footer>
  <div>
    <h3>Services</h3>
    {#each links as link}
      <a href="#0">{link}</a>
    {/each}
  </div>
  <div>
    <h3>Company</h3>
    {#each links2 as link}
      <a href="#0">{link}</a>
    {/each}
  </div>
  <div>
    <h3>Legal</h3>
    {#each links3 as link}
      <a href="#0">{link}</a>
    {/each}
  </div>
</footer>

<style>
  footer {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    padding: 5rem;
    align-items: center;
    background-color: var(--secondary-font-color);
    height: 20rem;
    margin-top: 2rem;
  }

  div {
    justify-self: center;
    align-self: baseline;
  }
  a {
    display: block;
    text-decoration: none;
    color: var(--footer-link);
    margin: 0.5rem 0;
  }
  h3 {
    color: #fff;
  }
</style>
