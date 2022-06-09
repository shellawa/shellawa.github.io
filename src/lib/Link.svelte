<script>
  export let data;
</script>

<a href={data.link} target="_blank">
  <div class="linkBox">
    <img draggable="false" src={"/assets/icons/" + data.icon} class="icon" alt="">
    <p class="name">{data.name}</p>
  </div>
</a>

<style>
  .linkBox {
    display: flex;
    align-content: space-between;
    justify-content: flex-start;
    align-items: center;
    background-color: #2f3136;
    box-shadow: 0 0.5rem 2rem rgb(0 0 0 / 5%);
    border-radius: 1rem;
    width: 100%;
    position: relative;
    padding: 0.5rem;
    margin-bottom: 2rem;
    min-width: 7rem;
    cursor: pointer;
  }
  .linkBox:hover {
    transform: scale(1.02);
  }
  .icon {
    min-width: 7rem;
    width: 7rem;
    height: 7rem;
    object-fit: cover;
  }
  .name {
    color: #fff;
    font-size: 1.6rem;
    margin: 0 1rem;
    line-height: 1.4;
    width: inherit;
    text-align: center;
  }
</style>
