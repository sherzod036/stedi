<template>
  <div class="page-categories page">
    <div class="container">
      <Breadcrumbs :crumbs="crumbs" />

      <span class="page_title">{{ $t('productTitle') }}</span>

      <div class="row section">
        <div
          v-for="category in categories"
          :key="category.id"
          class="col-md-6 col-lg-4"
        >
          <a :href="`categories/${category.slug}`" class="category">
            <span class="category__icon" v-html="category.icon"> </span>
            <span class="category__title">{{ category.title }}</span>
          </a>
        </div>
      </div>
    </div>
    <LayoutCatalog />

    <LayoutContacts />
  </div>
</template>

<script>
export default {
  async asyncData({ $axios, i18n }) {
    let langId = ''

    switch (i18n.locale) {
      case 'ru':
        langId = 1
        break
      case 'uz':
        langId = 2
        break
      case 'en':
        langId = 3
        break
      default:
        break
    }

    const config = {
      headers: {
        'X-LOCALE': langId
      }
    }

    const response = await $axios.$get('/categories', config)

    return { categories: response.data }
  },
  data() {
    return {
      crumbs: [
        {
          title: this.$t('mainTitle'),
          link: '/'
        },
        {
          title: this.$t('productTitle'),
          link: '#'
        }
      ]
    }
  }
}
</script>
