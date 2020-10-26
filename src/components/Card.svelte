<script>
  export let stay;
</script>

<div class="card">
  <img src={stay.photo} alt={stay.title}>
  <div class="info">
    <div class="left">
      {#if stay.superHost}
        <span class="badge">Super Host</span>
      {/if}
      <p>{stay.type}
        {#if stay.beds}
          {stay.beds} beds
        {/if}
      </p>
    </div>
    <div class="right">
      <p>{stay.rating}</p>
    </div>
  </div>
  <div class="desc">
    <p>{stay.title}</p>
  </div>
</div>

<style>
  .card {
    padding: 2rem;
    font-size: 14px;
  }

  .info {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .info .left {
    display: flex;
    align-items: center;
  }

  .info p {
    margin-left: 0.5rem;
    color: #828282;
  }

  .card .badge {
    border: 1px solid #4F4F4F;
    border-radius: 12px;
    width: 100px;
    font-size: 12px;
    font-weight: 700;
    text-transform: uppercase;
    padding: 0.3rem;
  }

  img {
    width: 395px;
    height: 295px;
    border-radius: 24px;
  }

  .desc p {
    font-size: 14px;
  }
</style>