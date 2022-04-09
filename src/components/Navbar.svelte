<script>
  import logo from "../assets/user.jpg"
</script>

<div class="nav">
  <div class="user">
    <img src={logo} alt="user" />
    <p>Y.Hoshino</p>
  </div>
  <p>Home</p>
  <p>About</p>
  <p>Works</p>
  <p>etc</p>
</div>

<style>
  .nav {
    flex:1;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;
    text-align: center;
    background: linear-gradient(
      to right bottom,
      rgba(255, 255, 255, 0.6),
        rgba(255, 255, 255, 0.1)
    );
    border-radius: 2rem;
  }

  .user img {
    width: 160px;
    height:160px;
    border-radius: 50%;
    border: 5px solid #fff;
    object-fit: cover;  /* この一行を追加するだけ！ */
  }
</style>