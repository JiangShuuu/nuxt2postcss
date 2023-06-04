<template>
  <div>
    <div class="block">
      <div class="block__element">
        <p class="block__element--modifier-title">Hello, BEM!</p>
        <p class="block__element--modifier-subtitle">Hello, SubBEM!</p>
      </div>
    </div>
    <div class="content">
      <div class="content__title_box">
        <div class="content__title">我是內容</div>
        <nuxt-link to="/">到 tailwind 頁面</nuxt-link>
      </div>
      <div class="content__container">
        <div class="menu">
          <div class="menu__item">選項 1</div>
          <div class="menu__item">選項 2</div>
          <div class="menu__item">選項 3</div>
          <div class="menu__item">選項 4</div>
        </div>
        <div class="card-container">
          <div class="card">
            <div class="card__contain">卡片內容</div>
            <h3 class="card__title">主標題 1</h3>
            <p class="card__subtitle">副標題 1</p>
            <img src="~/assets/img/heart.png" class="card__heart" />
          </div>
          <div class="card">
            <div class="card__contain">卡片內容</div>
            <h3 class="card__title">主標題 2</h3>
            <p class="card__subtitle">副標題 2</p>
            <img src="~/assets/img/heart.png" class="card__heart" />
          </div>
          <div class="card">
            <div class="card__contain">卡片內容</div>
            <h3 class="card__title">主標題 3</h3>
            <p class="card__subtitle">副標題 3</p>
            <img src="~/assets/img/heart.png" class="card__heart" />
          </div>
          <div class="card">
            <div class="card__contain">卡片內容</div>
            <h3 class="card__title">主標題 4</h3>
            <p class="card__subtitle">副標題 4</p>
            <img src="~/assets/img/heart.png" class="card__heart" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Scss',
}
</script>

<style lang="postcss" scoped>
.block {
  width: 100%;
  height: 100%;
  &__element {
    background: #fbc3a7;
    text-align: center;

    &--modifier {
      &-title {
        font-size: 32px;
        margin-bottom: 24px;
      }

      &-subtitle {
        font-size: 24px;
        line-height: 2rem;
      }
    }
  }
}

.content {
  width: 100%;
  height: 100%;
  margin-top: 16px;

  &__title_box {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  &__title {
    font-size: 24px;
    line-height: 2rem;
    margin-bottom: 10px;
    text-align: center;
    margin-right: 8px;
  }

  &__container {
    display: flex;
    flex-wrap: wrap;
  }
}

.menu {
  width: 20%;
  background-color: #f2f2f2;
  padding: 10px;
  margin-right: 10px;
  margin-bottom: 20px;

  .menu__item {
    margin-bottom: 8px;
  }
}

.card-container {
  width: 80%;
  flex: 1;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 16px;
  justify-items: center;

  .card {
    width: 150px;
    margin-bottom: 20px;
    padding: 24px;
    background-color: #f2f2f2;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    position: relative;
  }
  .card__contain {
    width: 100px;
    height: 100px;
    text-align: center;
    background: blue;
    color: white;
  }

  .card__title {
    font-size: 18px;
    margin-bottom: 8px;
    transition: color 0.3s ease-in-out;
    &:hover {
      color: red;
    }
  }

  .card__subtitle {
    font-size: 14px;
    transition: color 0.3s ease-in-out;
    &:hover {
      color: blue;
    }
  }
  .card__heart {
    position: absolute;
    width: 16px;
    height: 16px;
    top: 6px;
    right: 4px;
  }
}

@media (min-width: 768px) {
  .block {
    &__element {
      &--modifier {
        &-title {
          font-size: 42px;
        }

        &-subtitle {
          font-size: 32px;
        }
      }
    }
  }
  .content {
    &__title {
      font-size: 32px;
    }
  }
  .card-container {
    grid-template-columns: repeat(3, 1fr);
  }
  .card__title {
    &:hover {
      color: #008000;
    }
  }
}
</style>
