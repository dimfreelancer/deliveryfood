<template>
  <h1 class="title">Список товаров</h1>

  <div class="products-wrapper">
    <div class="products-card">
      <div class="products-card__image">
        <img class="products-card__image-img" src="/src/assets/img/goods/image-1.jpg" alt="goods 1">
      </div>
      <div class="products-card__description">
        <div class="products-card__description-row">
          <h5 class="products-card__description--name">
            Калифорния лосось стандарт
          </h5>
        </div><!-- row -->

        <div class="products-card__description-row">
          <p class="products-card__description--text">
            Рис, лосось, авокадо, огурец, майонез, икра масаго, водоросли нори.
          </p>
        </div><!-- row -->

        <div class="products-card__description-row">
          <div class="products-card__description-controls">
            
            <button class="products-card__btn btn btn-primary" title="Открыть корзину с заказами">
              <span class="products-card-text">В корзину</span>
              <img class="products-card-img" src="/src/assets/img/icons/shopping-cart-light.svg" alt="light cart">
            </button>
            
            <span class="products-card__description-controls--price">
              250&nbsp;&#8381;
            </span>
          </div>
        </div><!-- row -->
      </div>
    </div> <!-- products-card -->
    
  </div>

  <div class="products-description">
    <p class="goods-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maxime illum magni quasi alias. Nemo magni alias consequuntur, dolorum quis magnam, minima eum repellat pariatur maxime amet numquam eveniet. Deleniti, exercitationem!</p>
    <p class="goods-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae alias delectus suscipit culpa. Maiores placeat, est delectus corporis inventore praesentium, esse, aspernatur odio quod expedita assumenda! Officia rerum dolor voluptatem? Lorem ipsum, dolor sit amet consectetur adipisicing elit. Odit cumque totam nam laboriosam non dolorem, magnam similique voluptates dolorum, cupiditate a itaque eos doloremque, delectus exercitationem placeat iste deserunt magni. Lorem, ipsum dolor sit amet consectetur adipisicing elit. Hic magnam iste maiores placeat ut, sint adipisci soluta unde officia eligendi, veritatis, expedita nihil laboriosam quas libero maxime odio excepturi? Velit.</p>
  </div>
</template>



<script>
export default {

}
</script>

<style>
/* * products */

.products {
	display: block;
}
.products-header {
	display: flex;
	align-items: center;
	justify-content: space-between;
	flex-wrap: wrap;
	gap: 30px;
}
.goods-header {
	display: flex;
	flex-direction: row;
	justify-content: start;
	align-items: stretch;
}

.products-header--title {
	color: #000;
	font-size: 36px;
	font-weight: 700;
}
.products-header--search {
	border: 1px solid #d9d9d9;
	border-radius: 2px;
	min-width: 306px;
	height: 34px;
	color: #d9d9d9; /* ? */
	background-color: #fff;
	padding: 5px 12px;
	outline: none;
}
.products-header--search:focus {
	outline: none;
	border: 1px solid #d9d9d9;
}
.products-header--search::placeholder {
	color: #bfbfbf;
	font-size: 16px;
	font-weight: 400;
	line-height: 24px;
}

.products-wrapper {
	margin-top: 44px;
	margin-bottom: 90px;
	display: flex;
	justify-content: flex-start;
	flex-wrap: wrap;
	gap: 24px;
}

@media (width < 991px) {
	.products-wrapper {
		justify-content: space-evenly;
	}
}


.products-card {
	border-radius: 7px;
	display: flex;
	flex-direction: column;
	min-height: 377px;
	box-shadow: 0 4px 12px 0 rgba(0, 0, 0, 0.05);
	background-color: #fff;
	overflow: hidden;
	border-radius: 7px;
	max-width: 384px;
	min-height: 413px;
	text-decoration: none;

	width: calc((100% - 48px) / 3);
}

@media (width <= 991px) {
	.products-card {
		width: calc((100% - 24px) / 2);
	}
}

@media (width <= 576px) {
	.products-card {
		width: 100%;
	}
}


.products-card__image {
	border-start-start-radius: 7px;
	border-start-end-radius: 7px;
}

.products-card__image-img {
	border-start-start-radius: 7px;
	border-start-end-radius: 7px;
	height: 100%;
	width: 100%;
}

.products-card__description {
	display: flex;
	flex-direction: column;
	padding: 20px 24px;
	gap: 10px;
}


.products-card__description-info {
	display: flex;
	align-self: stretch;
	align-items: center;
	justify-content: space-between;
	gap: 26px;
	gap: 18px;
}

.products-card__description-row {
	display: flex;
	align-items: center;
	align-self: stretch;
	justify-content: space-between;
}

.products-card__description--title {
	display: flex;
	align-items: center;
	align-self: stretch;
	justify-content: space-between;
	font-weight: 700;
	font-size: 24px;
	line-height: 1.33;
	color: #000;
}


.products-card__description-info--rating {
	font-weight: 700;
	font-size: 18px;
	color: #FFC107;
	display: flex;
	align-items: center;
	justify-content: space-between;
	gap: 7.5px;
}

.products-card__star {
	display: block;
	width: 18px;
	height: 18px;
	transform: translateY(-1px);
}

.products-card__description-info--price,
.products-card__description-info--group {
	font-size: 18px;
	line-height: 178%;
	color: #8c8c8c;
}

.products-card__description-info--price {
	transform: translateX(8px);
}

.products-card__description-info--group {
	transform: translateX(-8px);
}

/*
.products-card__description-info--group {
	display: block;
	position: absolute;
}
.products-card__description-info--group::before {
	position: relative;
	display: block;
	content: '';
	width: 5px;
	height: 5px;
	border-radius: 50%;
}
*/

.products-card__description--name {
	margin: 0;
	color: #000;
	font-size: 24px;
	font-weight: 400;
	line-height: 1.33;
}

.products-card__description--text {
	margin: 0;
	color: #8c8c8c;
	font-size: 18px;
	font-weight: 400;
}

.products-card__description-controls {
	display: flex;
	align-items: center;
	justify-content: flex-start;
	flex-wrap: wrap;
	row-gap: 10px;
	column-gap: 30px;
}

.products-card__description-controls--price {
	color: #000;
	font-size: 20px;
	font-weight: 700;
	line-height: 1.6;
}

</style>