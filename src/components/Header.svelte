<script>
  import Search from './Search.svelte';
</script>

<header class="header">
  <div>
    <img src="images/logo.png" alt="WindBnb logo" >
  </div>
  <Search/>
</header>

<style>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>