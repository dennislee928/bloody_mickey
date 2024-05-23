<template>
  <Navbar />
  <IndexCard />
  <div class="marquee-container">
  <div class="marquee-content">
    "Gosh, I just tried to make a sandwich, but I put the peanut butter on my shoe instead! Oh boy!"

"Well, would ya look at that! I just found a rubber ducky in my cereal! Haha, how did that get there?"

"Hot dog! I accidentally used shampoo as toothpaste this morning! My breath smells like strawberries!"

"Aw, shucks! I was trying to bake a cake, but I ended up with a pizza! How'd that happen?"

"Gee whiz! I thought I was planting flowers, but it turns out I was watering my socks! Haha!" </div>
</div>
</template>

<script setup></script>
<style>
.divider {
  width: 100%;
  height: 2px;
  background-color: black;
  margin: 10px 0; /* Adjust spacing as needed */
}
.title {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  font-family: "Old Newspaper Types", serif;
  margin: 5px;
}
.first-title {
  font-size: 100px;
}
.second-title {
  font-size: 60px;
}
/**marquee part */

.marquee-container {
  width: 100%;
  overflow: hidden;
  display: flex;
  font-size: x-large;
}

.marquee-content {
  display: inline-block;
  white-space: nowrap;
  animation: marquee 50s linear infinite;
}

.marquee-content2 {
  display: inline-block;
  white-space: nowrap;
  animation: marquee2 50s linear infinite;
}
.marquee-content3 {
  display: inline-block;
  white-space: nowrap;
  animation: marquee2 50s linear infinite;
}

@keyframes marquee {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-100%);
  }
}

@keyframes marquee2 {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-100%);
  }
}
@keyframes marquee3 {
  0% {
    transform: translateX(0);
  }
  100% {
    transform: translateX(-100%);
  }
}
</style>
