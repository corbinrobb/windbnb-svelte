<script>
  import Card from "./Card.svelte";
  import { stays } from "../stays";
</script>

<section>
  <h3>Stays In Finland</h3>
  <div class="stays-container">
    {#each stays as stay}
      <Card stay={stay}/>
    {/each}
  </div>
</section>

<style>
  h3 {
    text-align: left;
    font-size: 24px;
  }

  section {
    margin-top: 4rem;
  }

  .stays-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
</style>