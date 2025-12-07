<div align="center">

<!-- Title -->
<h2 style="color:#6a0dad;">🌙 Factorial Tree</h2>

<!-- Tree Canvas -->
<div style="
  background: #1a0033;
  width: 300px;
  height: 400px;
  border-radius: 16px;
  position: relative;
  overflow: hidden;
">

  <!-- Tree -->
  <div style="
    position: absolute;
    bottom: 0;
    left: 50%;
    width: 20px;
    height: 120px;
    background: #4b0082;
    transform: translateX(-50%);
    border-radius: 10px;
  "></div>

  <!-- Branches -->
  <div style="position:absolute; bottom:100px; left:50%; width:100px; height:10px; background:#5a189a; transform:translateX(-50%) rotate(25deg);"></div>
  <div style="position:absolute; bottom:100px; left:50%; width:100px; height:10px; background:#5a189a; transform:translateX(-50%) rotate(-25deg);"></div>

  <!-- Leaves -->
  <div class="leaf">🍃</div>
  <div class="leaf">🍃</div>
  <div class="leaf">🍃</div>

</div>

<!-- Falling leaves animation -->
<style>
.leaf {
  position: absolute;
  top: -20px;
  font-size: 20px;
  animation: fall 5s linear infinite;
}

.leaf:nth-child(1) {
  left: 30px;
  animation-delay: 0s;
}

.leaf:nth-child(2) {
  left: 130px;
  animation-delay: 1s;
}

.leaf:nth-child(3) {
  left: 230px;
  animation-delay: 2s;
}

@keyframes fall {
  0% { top: -20px; opacity: 0; }
  50% { opacity: 1; }
  100% { top: 380px; opacity: 0; transform: rotate(360deg); }
}
</style>

</div>
