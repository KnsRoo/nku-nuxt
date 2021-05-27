<template>
	<ul>
		<li v-for="(link, idx) in getLinks" :key="idx">
			<nuxt-link :to="'/' + link.path">{{ link.name }}</nuxt-link>
		</li>
	</ul>
</template>

<script>
import jsonData from '../data.json'

export default {
	data(){
		console.log(this.getLinks);
		return {};
	},
	computed: {
		getLinks() {
	      return jsonData.landings.map((item) => {
	        return {
	          name: item.title,
	          path: item.path
	        }
	      })
	    }
	}
};
</script>
