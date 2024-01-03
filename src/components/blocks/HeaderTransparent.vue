<template>
  <header class="header">
    <!-- ======================== header container ========================= -->
    <div class="header__container">
      <!-- ======================== nav ========================= -->
      <nav class="header__nav">
        <ul class="nav__list">
          <li class="list__link">
            <RouterLink to="/">home</RouterLink>
          </li>
          <li class="list__link">
            <RouterLink to="/about">about</RouterLink>
          </li>
          <li class="list__link">
            <RouterLink to="/video">video</RouterLink>
          </li>
          <li class="list__link">
            <RouterLink to="/contact">contact</RouterLink>
          </li>
        </ul>
      </nav>
      <!-- ======================== actions ========================= -->
      <div class="header__actions">
        <div class="actions__input">
          <input type="text" placeholder="search" />
          <button>
            <ui-icon-search />
          </button>
        </div>
        <div class="actions__shopping-cart">
          <ui-button-default><ui-icon-cart-empty /></ui-button-default>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import UiButtonDefault from '@/components/ui/UiButtonDefault.vue'
import UiIconSearch from '@/components/ui/UiIconSearch.vue'
import UiIconCartEmpty from '@/components/ui/UiIconCartEmpty.vue'
</script>

<style lang="scss" scoped>
.header {
  &__container {
    display: flex;
    justify-content: end;
    align-items: center;
    padding: 41px 0 44px;
  }

  &__nav {
    margin-right: 115px;
  }

  &__actions {
    display: flex;
    border-radius: 12px;
  }
}
.nav {
  &__list {
    display: flex;
    column-gap: 47px;
  }
}
.list {
  &__link {
    color: #4f5b4f;
    font-size: 18px;
    font-weight: 700;
  }
}
.actions {
  &__input {
    display: flex;
    align-items: center;
    margin-right: 24px;
    input {
      width: 287px;
      height: 40px;
      padding: 10px 16px;
      background: #fff;
    }
    input:focus {
      outline: none;
    }
  }

  &__shopping-cart {
  }
}

// .header {

//   &__nav {
//     margin-right: 115px;
//   }

//   &__actions {
//     display: flex;
//     // border-radius: 12px;
//   }
// }
// .nav {
//   &__list {
//     display: flex;
//     column-gap: 47px;
//   }
// }
// .list {
//   &__link {
//     color: #4f5b4f;
//     font-size: 18px;
//     font-weight: 700;
//   }
// }
// .actions {
//   &__input {
//     display: flex;
//     align-items: center;
//     margin-right: 24px;
//     input {
//       width: 287px;
//       height: 40px;
//       padding: 10px 16px;
//       background: #fff;
//     }
//     input:focus {
//       outline: none;
//     }
//   }

//   &__shopping-cart {
//   }
// }
</style>
