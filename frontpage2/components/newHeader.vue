<template>
  <div class="header-container">
    <!-- Left Section: Publication Info -->
    <div class="publication-info">
      <p>Supscription Information: 1866 237 937</p>
      <p>Archived Issue: Issue1 Issue2</p>
      <p>Weather</p>
      <p>galagalagala</p>
    </div>

    <!-- Center Section: Newspaper Name -->
    <div class="newspaper-name">
      <p>Arkham Asylum Issue</p>
    </div>

    <!-- Right Section: Daily Quote -->
    <div class="container">
      <div class="daily-quote">
        <p>A smile a day keeps your pain away.</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.header-container {
  display: flex;
  justify-content: space-between;
  height: 10vh; /* 10% of the viewport height */
}

.publication-info {
  width: 20%;
  font-family: "Old Newspaper Types", serif; /* Assuming you have this font available */
  font-size: 8px;
  /**/
  margin: 0;
  height: 5vh; /* 10% of the viewport height */

  top: 50%;
}

.newspaper-name {
  width: 60%;
  font-family: "Old Newspaper Types", serif;
  text-align: center;
  font-size: xx-large;
  /**/
  margin: 0;

  top: 100%;
}

.daily-quote {
  border: 1px solid black;
  text-align: center;
  font-family: "Old Newspaper Types", serif;
  font-size: xx-small;
  /**/
  margin: 0;
  margin-right: 25px;
  margin-top: 10px;
  top: 50%;
}
.newspaper-name,
.daily-quote .container {
  display: flex;
  align-items: center; /* Centers text vertically */
  justify-content: center; /* Centers text horizontally */
}
.container {
  width: 20%;
  display: flex;
  align-items: center; /* Centers text vertically */
  justify-content: center; /* Centers text horizontally */
}
</style>
