<template>
  <input
    :type="type"
    class="px-6 py-3 bg-blue-50 rounded-lg outline-none"
    :placeholder="placeHolder"
  />
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "input",
  props: {
      placeHolder: String,
      type: String
  }
};
</script>
