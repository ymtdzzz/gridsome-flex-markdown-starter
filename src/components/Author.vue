<template>
  <div style="display: contents">
    <g-link to="/">
      <g-image
        src="~/assets/img/author.jpeg"
        :alt="$static.metadata.siteName"
      ></g-image>
    </g-link>
    <h1>
      <a href="/">{{ $static.metadata.siteName }}</a>
    </h1>

    <p>{{ $static.metadata.siteDescription }}</p>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
	siteDescription
  }
}
</static-query>

<script>
export default {
  props: ["showTitle"],
};
</script>
