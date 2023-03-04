<template>
  <section class="fitlab_goods">
    <div class="card__product-container">
      <div class="trainers__title">
        {{ staticText.product.otherModel[actualLang.index] }}
        
            </div>
      </section>
</template>
        
<script>
  import { mapState } from 'vuex';
  import { staticText } from '../i18n';
</script>

  computed: {
    ...mapState({
      product: (state) => state.products.product,
      actualLang: (state) => state.settings.actualLang,
    }),
