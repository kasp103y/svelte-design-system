<script>
  export let title;
  import Badge from "./Badge.svelte";
  import Button from "./Button.svelte";
</script>

<article>
  <img src="./sko.jpg" alt="Sko" />
  <div class="card-indhold">
    <h3>{title} <Badge type="secondary">NEW</Badge></h3>

    <p>If a dog chews shoes whose shoes does he choose</p>
    <div class="badges">
      <Badge type="border">Fashion</Badge>
      <Badge type="border">Products</Badge>
    </div>

    <div class="card-btn"><Button type="primary">Buy now</Button></div>
  </div>
</article>

<style>
  article {
    border-radius: 1rem;
    box-shadow: rgba(136, 165, 191, 0.48) 6px 2px 16px 0px,
      rgba(255, 255, 255, 0.8) -6px -2px 16px 0px;
    display: flex;
    flex-direction: column;
    width: 20rem;
  }

  img {
    aspect-ratio: 16/9;
    object-fit: cover;
    border-radius: 1rem 1rem 0 0;
  }

  .card-indhold {
    padding: 0.5rem 1rem;
  }

  .card-btn {
    text-align: end;
    margin-top: 0.5rem;
  }

  .badges {
    margin: 1rem 0;
  }
</style>
