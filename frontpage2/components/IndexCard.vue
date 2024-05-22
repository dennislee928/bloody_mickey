<template>
  <div class="background-image">
    <img src="../assets/evil mickey.jpeg" class="evil-mickey" />
    <div class="overlay">
      <div class="main-title">
        <p>You don’t!</p>
        <p>F*cking!</p>
        <p>Talk to me like that!</p>
        <p>Ha-ha.</p>
      </div>
      <div class="fun-market">
        <a href="https://crypto.com/price/mickey-mouse">
          <button class="buy">Buy mickey crypto</button>
        </a>

        <div class="twitter">
          <a href="https://x.com/evil_mickey?lang=zh-Hant">X</a>
        </div>
        <div class="wiki"></div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.background-image {
  position: relative;
  width: 100%;
  height: 100vh; /* Full viewport height */
  overflow: hidden;
}

.evil-mickey {
  width: 100%;
  height: 100vh; /* Full viewport height */
  object-fit: cover; /* Ensures the image covers the area without distorting */
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: aliceblue;
}

.main-title {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  font-size: 2rem; /* Responsive font size */
  z-index: 10;
  padding: 20px;
  background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent background */
  height: auto;
}

.fun-market {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 20px;
}

.sub-title {
  padding: 20px;
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  background-color: rgba(0, 0, 0, 0.5); /* Semi-transparent background */
}

.buy {
  font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
  background-color: darkblue;
  color: white;
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  margin-top: 10px;
}
</style>
