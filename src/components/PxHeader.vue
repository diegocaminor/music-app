<template lang="pug">
  .container
    .header
      a.header__thumbnail
        img.header__img(src="@/assets/images/movie-logo.png")
      input.input.header__input
      div.label.header__user
        img.label.header__user--username
        label.label.header__user--image
</template>

<script>
export default {
  name: "PxHeader"
};
</script>

<style lang="scss" scoped>
// .header__img {
//   height: 200px;
// }
</style>