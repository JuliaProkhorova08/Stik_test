<template>
  <div>
    <Header />
    <Card />
    <Nuxt />
  </div>
</template>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
}

html {
  box-sizing: border-box;
  height: 100%;
}

body {
  display: flex;
  flex-direction: column;
  min-width: 375px;
  min-height: 100%;
  margin: 0 auto;
  background-color: #fff;
}

img {
  max-width: 100%;
  height: auto;

  object-fit: scale-down;
}
</style>
