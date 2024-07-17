<template>
    <li>
      {{ node.name }}
      <ul v-if="node.children">
        <tree-node v-for="(child, index) in node.children" :key="index" :node="child"></tree-node>
      </ul>
    </li>
  </template>
  
  <script setup>
  import { defineProps } from 'vue';
  
  const props = defineProps({
    node: Object
  });
  </script>
  
  <style scoped>
  /* Your TreeNode styles here */
  </style>
  