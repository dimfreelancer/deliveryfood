<template>
<!-- footer bgn -->
<footer class="footer">
  <div class="container">
    <div class="footer-box">
      <a class="footer-logo logo" href="/">
        <img class="footer-logo-image" src="/src/assets/img/logo/logo.svg" alt="logo delivery food" title="logo delivery food png">
      </a>
      
      <nav class="footer-nav nav">
        <ul class="nav-list">
          <li class="nav-item">
            <a class="nav-link" href="/restraunts" title="Список наших ресторанов">Ресторанам</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/couries" title="Информация для курьеров и доставки">Курьерам</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/press" title="Пресс центр для прессы">Пресс-центр</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/contacts" title="Наши контакты">Контакты</a>
          </li>
        </ul>
      </nav>
      
      <div class="footer-social social">
        <ul class="social-list">
          <li class="social-item">
            <a class="social-link" href="#">
              <img class="footer-image" src="/src/assets/img/social/ins.svg" alt="inst">
            </a>
          </li>
          
          <li class="social-item">
            <a class="social-link" href="#">
              <img class="footer-image" src="/src/assets/img/social/fb.svg" alt="face">
            </a>
          </li>
          
          <li class="social-item">
            <a class="social-link" href="#">
              <img class="footer-image" src="/src/assets/img/social/vk.svg" alt="vk vkontakte" title="Перейти в наш паблик вКонтакте">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</footer>
<!-- footer end -->
</template>

<script>
export default {

}
</script>



<style>

/* * FOOTER */

.footer {
	display: flex;
	justify-content: center;
	align-items: center;
  min-height: 156px;
	padding-top: 60px;
	padding-bottom: 60px;
	padding: 60px 0;
}

.footer-box {
  width: 100%;
	height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
	gap: 36px;
	flex-wrap: wrap;
}

.footer-nav {
	display: flex;
	flex-grow: 1;
}

.nav-list {
	display: flex;
	justify-content: space-between;
	align-items: center;
	list-style: none;
	padding: 0;
	margin: 0;
	gap: 15px;
	flex-wrap: wrap;
}
.nav-item {
	color: #595959;
	font-family: Roboto, sans-serif;
	font-size: 18px;
	font-style: normal;
	font-weight: 400;
	line-height: normal;
}

.social-list {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}
.social-item {
	display: block;
}

</style>
