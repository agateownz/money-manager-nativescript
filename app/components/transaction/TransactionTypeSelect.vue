<template>
  <DropDown
    :items="items"
    :selectedIndex="selectedType"
    class="item-drop-down"
    @selectedIndexChanged="$emit('typeSelected', $event)"
  />
</template>

<script>
export default {
  data() {
    return {
      items: ['Despesas', 'Renda'],
      selectedType: 0,
    };
  },
};
</script>

<style lang="scss" scoped>
.item-drop-down {
  horizontal-align: left;
  font-size: 18;
  margin: 8 8;
  padding: 6 16;
  height: 40;
}
</style>
