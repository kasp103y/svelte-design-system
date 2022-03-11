<script>
  export let name;
  export let type = "default";
  export let mode = "default";
  export let image = true;
</script>

<div class="container {type}">
  <div class:indicator={mode === "indicator"} />
  <div />

  {#if image === true}
    <img src="./sko.jpg" alt="" />
  {:else}
    <p>{name}</p>
    <p />{/if}
</div>

<style>
  .container {
    background-color: var(--secondary-font-color);
    border-radius: 100%;
    border: 4px solid var(--secondary-font-color);
    display: flex;
    width: 4rem;
    height: 4rem;
    color: white;
    justify-content: center;
    align-items: center;
    position: relative;
    font-size: 2rem;
  }

  img {
    height: 100%;
    width: 100%;
    border-radius: 100%;
  }

  .indicator {
    width: 15%;
    height: 15%;
    background-color: greenyellow;
    border: 1px solid #fff;
    border-radius: 100%;
    position: absolute;
    top: 5%;
    right: 3%;
  }

  .large {
    width: 8rem;
    height: 8rem;
    font-size: 2rem;
  }

  .medium {
    width: 6rem;
    height: 6rem;
    font-size: 1.5rem;
  }

  .small {
    width: 4rem;
    height: 4rem;
    font-size: 1rem;
  }
</style>
