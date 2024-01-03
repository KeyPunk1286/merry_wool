<template>
  <div class="footer">
    <div class="footer__link">
      <ul class="link__list">
        <li><img src="@/assets/icons/facebook_logo.png" alt="" /></li>
        <li><img src="@/assets/icons/insta_logo.png" alt="" /></li>
        <li><img src="@/assets/icons/telegram_logo.png" alt="" /></li>
      </ul>
    </div>
    <div class="footer_nav">
      <ul class="nav__list">
        <li><RouterLink to="/">home</RouterLink></li>
        <li><RouterLink to="/about">about</RouterLink></li>
        <li><RouterLink to="/video">video</RouterLink></li>
        <li><RouterLink to="/contact">contact</RouterLink></li>
      </ul>

      <div class="nav__text">© 2021 Candy yarn. All rights reserved.</div>
    </div>

    <div class="footer__contact">
      <div class="contact__tel">+38093 567 85 43</div>
      <div class="contact__email">candyyarn@gmail.com</div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.footer {
  max-width: 1119px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  &_nav {
  }

  &__link {
  }

  &__contact {
  }
}
.link {
  &__list {
    display: flex;
  }
}
.nav {
  &__list {
    display: flex;
  }

  &__text {
  }
}
.contact {
  &__tel {
  }

  &__email {
  }
}
</style>
