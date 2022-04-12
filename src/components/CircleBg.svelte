

<div class="circle1"></div>
<div class="circle2"></div>
<div class="circle3"></div>


<style>
.circle1,
.circle2,
.circle3 {
  background: white;
  background: linear-gradient(
    to right bottom,
    rgba(255, 255, 255, 0.9),
      rgba(255, 255, 255, 0.3)
  );
  position: absolute;
  border-radius: 50%;
}

.circle1{
  top: 5%;
  right: 15%;
  height: 15rem;
  width: 15rem;
}

.circle2{
  bottom: 3%;
  left: 35%;
  height: 10rem;
  width: 10rem;
  animation: zoomInOut 8s linear infinite;
  background-color: rgb(255, 157, 45);
}

.circle3{
  top: 35%;
  left: 30%;
  height: 5rem;
  width: 5rem;
  background-color: rgb(50, 122, 255);
}
/* @keyframes zoomInOut{
  0%, 100%{
    transform: scale(0.5);
  }
  50% {
    transform: scale(1)
  }
} */

  </style>