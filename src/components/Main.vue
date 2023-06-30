<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})
 
</script>

<template>
  <h1>{{ msg }}</h1>
  <menu-section></menu-section>
</template>

<script>
Vue.component('menu-section', {
	template: '<ul><li v-for="item in menuItems">{{ item.text }}</li></ul>',
	data: function() {
		return {
			menuItems: [{
			    text: 'About me'
			}, {
			    text: 'Articles'
			}, {
			    text: 'contact'
			}]
		};
	}
});
</script>


<style scoped>
.read-the-docs {
  color: #888;
}
</style>
