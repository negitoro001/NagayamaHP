<template>
  <div>

    <section class="main-content columns">
      <aside class="column is-2 section">
        <b-sidebar
          type="is-success"
          :overlay="overlay"
          :right="right"
          v-model="open"
          position="fixed"
          :fullheight="fullheight"
        >
          <b-menu>
            <b-menu-list>
              <b-menu-item
                icon="arrow-left-top-bold"
                label="トップページ"
              />
              <b-menu-item
                icon="text-account"
                label="略歴"
              />
              <b-menu-item
                icon="information-outline"
                label="ブログ"
              />
              <b-menu-item
                icon="form-select"
                label="問い合わせフォーム"
              />
            </b-menu-list>
          </b-menu>
        </b-sidebar>
      </aside>

      <div class="container column is-10">
        <Nuxt />
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fullheight: true,
      overlay: false,
      right: false,
      open: true,
    };
  },
};
</script>
