<template>
  <span>Posted at {{ post.date }} • <g-link :to="post.category.path" v-html="post.category.title"></g-link></span>
</template>

<script>
export default {
  props: ['post'],
}
</script>
