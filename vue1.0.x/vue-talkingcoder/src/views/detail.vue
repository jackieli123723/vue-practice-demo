<template>
	<div>
		<me-header-tab title="详情页" router="/home"></me-header-tab>
        <div class="me-container">
        	<h3>详情页</h3>
        	<p>{{Lcontent}}</p>
        </div>
   	</div>
</template>
<script>
import MeHeaderTab from './me/MeHeaderTab.vue';
	export default {
		route: {
		  data: function (transition) {

		   this.$set('Lcontent',decodeURIComponent(this.$route.params.Lcontent));
		  }
		},
		ready (){
		     $.init();

		  },
		data (){
			return {
				Lcontent : ''
			}
		},
		components:{
				MeHeaderTab
		}
	}
</script>


<style scoped>
	h3{
		text-align: center;
	}
	p{
		background: #fff;
		padding: 2rem 0.5rem;
	}
</style>
