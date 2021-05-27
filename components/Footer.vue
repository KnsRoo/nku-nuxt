<template>
  <footer class="footer">
    <div class="footer__container">
      <a class="footer__company" href="/">NKU</a>
      <a class="footer__phone" href="tel:+79164441159">+7-916-444-11-59</a>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style>
.footer {
  padding: 2px 0;
  background-color: #026aa7;
  justify-content: center;
}

.footer__container {
  display: flex;
  overflow: hidden;
  justify-content: space-between;
  align-items: center;
  width: 1120px;
  padding: 0 10px;
}

.footer__company {
  color: #fff;
  font-size: 3rem;
  text-decoration: none;
}

.footer__company:hover {
  color: #fff;
  text-decoration: none;

}

.footer__right {
  align-items: center;
}

.footer__email {
  color: #fff;
  font-size: 1.5rem;
  text-decoration: none;
}

.footer__phone {
  color: #fff;
  font-size: 1.75rem;
  margin-left: 40px;
  text-decoration: none;
}

@media (max-width: 576px) {
  .footer__container {
    flex-direction: column;
  }

  .footer__phone {
    margin-left: 0;
    margin-top: 10px;
  }
}
</style>