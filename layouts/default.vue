<template>
  <div
    id="app"
    class="container"
  >
    <section>
      <b-sidebar
        type="is-light"
        :overlay="overlay"
        :right="right"
        v-model="open"
        :fullheight="fullheight"
      >
        <b-menu>
          <b-menu-list>
            <b-menu-item
              icon="arrow-left-top-bold"
              label="トップページ"
            ></b-menu-item>
            <b-menu-item
              icon="text-account"
              label="略歴"
            ></b-menu-item>
            <b-menu-item
              icon="information-outline"
              label="ブログ"
            ></b-menu-item>
            <b-menu-item
              icon="form-select"
              label="問い合わせフォーム"
            ></b-menu-item>
          </b-menu-list>
        </b-menu>
      </b-sidebar>

    </section>
    <div class="p-1">
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fullheight: true,
      fullwidth: true,
      overlay: false,
      right: false,
      open: true,
    };
  },
};
</script>
