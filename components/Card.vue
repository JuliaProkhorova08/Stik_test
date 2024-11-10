<template>
  <div class="card">
    <picture class="card__photo">
      <source
        media="(min-width: 1440px)"
        srcset="
          ~assets/img/card-desktop-01@1x.jpg 1x,
          ~assets/img/card-desktop-01@2x.jpg 2x
        "
        sizes="518px"
      />
      <img
        src="~assets/img/card-mobile-01@1x.jpg"
        width="375"
        height="617"
        alt="Фото девушки в белом жакете."
      />
    </picture>
  </div>
</template>

<style>
.card__photo {
  display: flex;
  justify-content: center;
  width: 100%;
}

.card__photo img {
  max-width: 100%;
  height: auto;
}
</style>
