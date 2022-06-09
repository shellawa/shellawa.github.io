<script>
  export let data;
</script>

<section class="headerBox">
  <section class="header">
    <div class="pfp">
      <img src={"/assets/pfps/" + data.avatarUrl} alt="pfp" srcset="" />
    </div>
    <div>
      <div class="name">
        <h1>{data.name}</h1>
      </div>
      <div class="bio">
        <p>{data.bio}</p>
      </div>
    </div>
  </section>
</section>

<style>
  .headerBox {
    padding: 2rem 2rem 1rem;
    background-color: #2f3136;
    box-shadow: 0 0.5rem 2rem rgb(0 0 0 / 5%);
  }
  @media screen and (min-width: 0px) {
    .headerBox {
      border-radius: 0 0 1rem 1rem;
    }
  }
  @media screen and (min-width: 768px) {
    .headerBox {
      border-radius: 1rem;
    }
  }
  .header {
    display: flex;
    align-items: center;
    position: relative;
  }
  .pfp {
    margin-right: 2rem;
    min-width: 6rem;
    min-height: 6rem;
    border-radius: 50rem;
  }
  .pfp img {
    border-radius: 50%;
    max-width: 6rem;
  }
  .name {
    display: flex;
    align-items: center;
  }
  @media screen and (min-width: 0) {
    .name {
      font-size: 1.8rem;
    }
  }
  @media screen and (min-width: 350px) {
    .name {
      font-size: 2rem;
    }
  }
  .bio {
    color: #726b8c;
    font-size: 1.4rem;
    opacity: 0.6;
  }
</style>
