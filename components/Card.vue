<template>
<div class="hero">
  <ul class="hero__gallery gallery">
    <li class="gallery__item gallery__item--active">
      <img
        src="~assets/img/gallery-desktop-01@1x.jpg"
        width="70"
        height="88"
        alt="Фото девушки в белом жакете."
      />
    </li>
    <li class="gallery__item">
      <img
        src="~assets/img/gallery-desktop-02@1x.jpg"
        width="70"
        height="88"
        alt="Фото девушки в белом жакете."
      />
    </li>
    <li class="gallery__item">
      <img
        src="~assets/img/gallery-desktop-03@1x.jpg"
        width="70"
        height="88"
        alt="Фото девушки в белом жакете."
      />
    </li>
  </ul>

  <div class="hero__card card">
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

  <div class="hero__container">

  <div class="hero__wrapper">

    <div class="hero__info">
      <ul class="hero__list">
    <li class="hero__item hero__item--text">
      жакет удлинённый, белый
    </li>
    <li class="hero__item">
      8900 RUB
    </li>
      </ul>
      <picture class="hero__fav">
    <svg width="14" height="18" viewBox="0 0 14 18" fill="none" xmlns="http://www.w3.org/2000/svg">
<path fill-rule="evenodd" clip-rule="evenodd" d="M1 0H14V17.4819L7.51338 13.1182L1 17.4819V0ZM2 1V15.5181L7.51338 11.8818L13 15.5181V1H2Z" fill="#333333"/>
</svg>

      </picture>
    </div>

  </div>

  <div class="hero__size">
    <p>Размеры</p>

    <div class="hero__sizes">
      <p class="hero__sizes hero__sizes--item">XS</p>
      <p class="hero__sizes hero__sizes--item">S</p>
      <p class="hero__sizes hero__sizes--item">M</p>
    </div>
    <div class="hero__sizestext">
      <p class="hero__sizestext hero__sizestext--item">мало</p>
      <p class="hero__sizestext hero__sizestext--item">подписка</p>
    </div>

  </div>

  <div class="hero__color">
    <p>Цвет: белый</p>

    <div class="hero__colors">
      <span class="hero__colors hero__colors--white"></span>
      <span class="hero__colors hero__colors--black"></span>
      <span class="hero__colors hero__colors--beige"></span>
    </div>
  </div>

  <div class="hero__buy">
    <button>Добавить в корзину</button>
    <picture>
      <svg width="44" height="44" viewBox="0 0 44 44" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect x="0.5" y="0.5" width="43" height="43" stroke="black"/>
<path fill-rule="evenodd" clip-rule="evenodd" d="M15.5 14H28.5V31.4819L22.0134 27.1182L15.5 31.4819V14ZM16.5 15V29.5181L22.0134 25.8818L27.5 29.5181V15H16.5Z" fill="black"/>
</svg>
    </picture>
  </div>

  <ul class="hero__description description">
    <li class="description__item">
      <button class="description__item description__item--button">Описание</button>
    </li>
    <li class="description__item">
      <button class="description__item description__item--button">Состав и уход</button>
    </li>
  </ul>
</div>
</div>
</template>

<style>
.hero {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;

  @media (min-width: 1440px) {
    flex-direction: row;
  }

}

.hero__gallery {
  display: none;

  @media (min-width: 1440px) {
    display: flex;
    flex-direction: column;
    margin: 0;
    margin-right: 30px;

    list-style: none;
  }
}

.card__photo {
  width: 100%;
}

.card__photo img {
  max-width: 100%;
  height: auto;
}

.hero__wrapper {
  padding: 0 16px;
}

.hero__info {
  display: flex;
  justify-content: space-between;
  margin-top: 26px;
  margin-bottom: 36px;

  @media (min-width: 1440px) {
    margin-top: 0;
    margin-bottom: 31px;
  }
}

.hero__list {
  margin: 0;
  padding: 0;

  list-style: none;
}

.hero__item {
  font-size: 12px;
  line-height: 16px;
  color: #333333;
  text-transform: uppercase;
}

.hero__item--text {
  margin-bottom: 8px;
}

.hero__fav {
  @media (min-width: 1440px) {
    display: none;
  }
}

.hero__size {
  padding-right: 16px;
  padding-left: 16px;
}

.hero__size p {
  margin: 0;
  margin-bottom: 9px;
  font-size: 10px;
  line-height: 14px;
  color: #4f4f4f;

  @media (min-width: 1440px) {
    margin-bottom: 8px;
  }
}

.hero__sizes {
  display: grid;
align-items: center;
margin-bottom: 4px;
padding: 0;

font-size: 10px;
line-height: 14px;
text-align: center;

grid-column-gap: 9px;
grid-row-gap: 0;
grid-template-columns: repeat(3, 65px);
grid-template-rows: 31px;
}

.hero__sizes--item {
  margin: 0;
}

.hero__sizes--item:nth-child(1),
.hero__sizes--item:nth-child(2) {
  color: #333333;

  border: 1px #333333 solid;
}

.hero__sizes--item:nth-child(3) {
  color: #bdbdbd;

  border: 1px #bdbdbd solid;
}

.hero__sizestext {
  display: flex;
  justify-content: space-between;
height: 18px;
  margin: 0;
  margin-bottom: 34px;

  @media (min-width: 1440px) {
    margin-bottom: 36px;
  }
}

.hero__sizestext--item:nth-child(1) {
  padding-left: 20px;

  color: #828282;
}

.hero__sizestext--item:nth-child(2) {
  padding-right: 140px;

  color: #bdbdbd;
}

.hero__color {
  margin-bottom: 32px;
  padding: 0 16px;

  @media (min-width: 1440px) {
    margin-bottom: 36px;
  }
}

.hero__color p {
  margin: 0;
  margin-bottom: 6px;

  font-size: 10px;
  line-height: 14px;
  color: #4f4f4f;
}

.hero__colors {
  display: flex;
  width: 116px;
  height: 27px;

  gap: 16px;
}

.hero__colors--white {
  background-color: #ffffff;
  border:#bdbdbd 1px solid;
}

.hero__colors--white::after {
  content: "";

  display: block;
  width: 28px;
  height: 1px;
  margin-top: 31px;

  background-color: #4f4f4f;

}

.hero__colors--black {
  background-color: #000000;
}

.hero__colors--beige {
  background-color: #f9f1dc;
}

.hero__buy {
  display: none;

  @media (min-width: 1440px) {
    display: grid;
    grid-template-columns: 290px 44px;
grid-template-rows: 44px;
grid-column-gap: 10px;
grid-row-gap: 0px;
padding: 0 16px;
margin-bottom: 40px;
  }
}

.hero__buy button {
  padding: 0;
  font-size: 11px;
  line-height: 15px;
  text-transform: uppercase;
  color: #fff;
  background-color: #000000;
}

.hero__description {
  padding: 0 16px;
  margin: 0;
  margin-bottom: 40px;
  list-style: none;
}

.description__item {
  margin: 0;
display: flex;
justify-content: space-between;
align-items: center;
}

.description__item--button {
  position: relative;
  width: 343px;
  height: 41px;
  border: none;
  border-bottom: 1px #E0E0E0 solid;
  background-color: transparent;
  text-align: left;
  text-transform: uppercase;
  font-size: 10px;
  line-height: 14px;
  color: #333333;
}

.description__item--button::before,
.description__item--button::after {
position: absolute;
content: "";
background-color: #828282;
    width: 9px;
    height: 9px;
}

.description__item--button::before {
width: 10px;
    height: 1px;
    top: 50%;
    right: 9px;
    transform: translateY(-50%);
}

.description__item--button::after {
width: 1px;
    height: 10px;

    right: 13px;
    transform: translateX(-50%);
}

.description__item:nth-child(1) .description__item--button {
  padding: 0;
  border-top: 1px #E0E0E0 solid;
}

.description__item:nth-child(2) .description__item--button {
  padding: 0;
  border-top: none;
}


</style>
