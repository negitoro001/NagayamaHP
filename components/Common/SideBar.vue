<template>
  <b-sidebar
    type="is-light"
    :right="right"
    :fullheight="fullheight"
    v-model="activeModel"
    open
  >
    <b-menu>
      <b-menu-list>
        <b-menu-item
          active
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
</template>

<script>
export default {
  data() {
    return {
      activeModel: "",
      fullheight: true,
      right: false,
    };
  },
};
</script>
