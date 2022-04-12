<script>
  import { onMount } from 'svelte';

  onMount( ()=> {
    let themeColor = document.querySelectorAll('.theme span');
    console.log(themeColor)
    
    themeColor.forEach(color => color.addEventListener('click', ()=>{
    let background = color.style.background;
    document.querySelector('.main').style.background = background;
  }));
  })

</script>

<div class="theme animate__animated animate__bounceInUp animate__slower">
  <span class="base"></span>
  <span style="background: linear-gradient(deeppink, purple);"></span>
  <span style="background: linear-gradient(lightgreen, crimson);"></span>
  <span style="background: linear-gradient(#999, #111);"></span>
</div>

<style>
.theme{
  background: white;
  min-height: 40vh;
  width:5%;
  margin-left: 15px;
  background: linear-gradient(
    to right bottom, 
  rgba(255, 255, 255, 0.7),
  rgba(255, 255, 255, 0.2)
  );
  border-radius: 1rem;
  backdrop-filter:blur(1rem);
}
.theme span{
  display: block;
  height: 2rem;
  width: 2rem;
  border-radius: 50%;
  margin: 10px auto;
  cursor: pointer;
}


span.base{
  background: rgba(255, 255, 255, 0.7);
}
</style>