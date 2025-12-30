<div align="center">

<h1 class="glitch" data-text="Hi there! 👋">Hi there! 👋</h1>

<h2 class="name">I am Muhammad Eman</h2>

<p class="quote glitch" data-text="Code builds the product, and strategy builds the growth.">
  Code builds the product, and strategy builds the growth.
</p>

</div>

<style>
.glitch {
  position: relative;
  color: #fff;
  font-weight: bold;
  animation: glitch 1.5s infinite;
}

.glitch::before,
.glitch::after {
  content: attr(data-text);
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  overflow: hidden;
}

.glitch::before {
  color: #00fff9;
  animation: glitchTop 1.5s infinite linear;
}

.glitch::after {
  color: #ff00c1;
  animation: glitchBottom 1.5s infinite linear;
}

@keyframes glitch {
  0% { transform: none; }
  20% { transform: skew(-5deg); }
  40% { transform: skew(5deg); }
  60% { transform: skew(-3deg); }
  80% { transform: skew(3deg); }
  100% { transform: none; }
}

@keyframes glitchTop {
  0% { clip-path: inset(0 0 80% 0); transform: translate(-2px, -2px); }
  50% { clip-path: inset(10% 0 60% 0); transform: translate(2px, 2px); }
  100% { clip-path: inset(0 0 80% 0); transform: translate(-2px, -2px); }
}

@keyframes glitchBottom {
  0% { clip-path: inset(80% 0 0 0); transform: translate(2px, 2px); }
  50% { clip-path: inset(60% 0 10% 0); transform: translate(-2px, -2px); }
  100% { clip-path: inset(80% 0 0 0); transform: translate(2px, 2px); }
}

body {
  background-color: #0d1117;
}

.name {
  color: #58a6ff;
  margin-top: -10px;
}

.quote {
  font-size: 18px;
  margin-top: 10px;
}
</style>
