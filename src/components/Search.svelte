<script>
  let location = 'Helsinki, Finland';
  let guests = '';
</script>

<div class="search">
  <input
    class="input"
    bind:value={location}
    placeholder="Location"
  />
  <input
    class="input"
    bind:value={guests}
    placeholder="Add guests"
  />
  <button>Search</button>
</div>

<style>
  .search {
    border-radius: 1rem;
    box-shadow: 0px 1px 6px rgba(0, 0, 0, 0.1);
    display: flex;
    height: 3rem;
  }

  .input {
    border: none;
    border-top-left-radius: 1rem;
    border-bottom-left-radius: 1rem;
    height: 100%;
    border-right: solid 1px rgba(0, 0, 0, 0.1);
    text-align: center;
    font-size: 14px;
  }

  ::placeholder {
    color: #BDBDBD;
  }

  button {
    height: 100%;
    border-top-right-radius: 1rem;
    border-bottom-right-radius: 1rem;
    background-color: #fff;
    color: #EB5757;
    border: none;
  }
</style>