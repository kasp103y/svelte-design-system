<script>
  import Button from "./Button.svelte";
  import Badge from "./Badge.svelte";
  export let title;
  export let number;
</script>

<div class="container">
  <Button
    >{title}
    <div class="element"><Badge type="secondary">{number}</Badge></div></Button
  >
</div>

<style>
  .container {
    position: relative;
    display: inline-block;
  }

  .element {
    position: absolute;
    top: -15%;
    right: -10%;
  }
</style>
