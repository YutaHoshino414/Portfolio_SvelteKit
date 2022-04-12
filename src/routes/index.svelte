<script>
import Navbar from "../components/Navbar.svelte";
import global from  "../global.css"
import 'animate.css';
import CircleBg from "../components/CircleBg.svelte";
import ThemeBar from "../components/ThemeBar.svelte";
</script>

<div class="main">
  <div class="glass animate__animated animate__rotateIn "> 
    <Navbar />
    <div class="content">dd</div>
  </div>
  <ThemeBar />
  <CircleBg />
</div>


<style>
.main{
  min-height: 100vh;
  background-color: #FAFFB7; 
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 1200 800'%3E%3Cdefs%3E%3CradialGradient id='a' cx='0' cy='800' r='800' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%23fde285'/%3E%3Cstop offset='1' stop-color='%23fde285' stop-opacity='0'/%3E%3C/radialGradient%3E%3CradialGradient id='b' cx='1200' cy='800' r='800' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%235cff72'/%3E%3Cstop offset='1' stop-color='%235cff72' stop-opacity='0'/%3E%3C/radialGradient%3E%3CradialGradient id='c' cx='600' cy='0' r='600' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%234cfc2b'/%3E%3Cstop offset='1' stop-color='%234cfc2b' stop-opacity='0'/%3E%3C/radialGradient%3E%3CradialGradient id='d' cx='600' cy='800' r='600' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%23FAFFB7'/%3E%3Cstop offset='1' stop-color='%23FAFFB7' stop-opacity='0'/%3E%3C/radialGradient%3E%3CradialGradient id='e' cx='0' cy='0' r='800' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%23FAA454'/%3E%3Cstop offset='1' stop-color='%23FAA454' stop-opacity='0'/%3E%3C/radialGradient%3E%3CradialGradient id='f' cx='1200' cy='0' r='800' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%230CF'/%3E%3Cstop offset='1' stop-color='%230CF' stop-opacity='0'/%3E%3C/radialGradient%3E%3C/defs%3E%3Crect fill='url(%23a)' width='1200' height='800'/%3E%3Crect fill='url(%23b)' width='1200' height='800'/%3E%3Crect fill='url(%23c)' width='1200' height='800'/%3E%3Crect fill='url(%23d)' width='1200' height='800'/%3E%3Crect fill='url(%23e)' width='1200' height='800'/%3E%3Crect fill='url(%23f)' width='1200' height='800'/%3E%3C/svg%3E");
  background-attachment: fixed;
  background-size: cover;
  display:flex;
  align-items: center;
  justify-content: center;
}

.glass {
  background: white;
  min-height: 80vh;
  width:85%;
  background: linear-gradient(
    to right bottom, 
  rgba(255, 255, 255, 0.7),
  rgba(255, 255, 255, 0.2)
  );
  border-radius: 2rem;
  backdrop-filter:blur(1rem);
  z-index: 2;
  display:flex;
}

.content {
  flex:3;
}

</style>