<template>
	<div class="tab-control">
		<div class="tab-control-item"
				 v-for="(item, index) in titles"
				 :class="{active: index === currentIndex}"
				 @click="itemClick(index)">
			<span>{{item}}</span>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'TabControl',
		props: {
			titles: {
				type: Array,
				default() {
					return []
				}
			}
		},
		data() {
			return {
				currentIndex: 0
			}
		},
		methods: {
			itemClick(index) {
				this.currentIndex = index
				this.$emit('tabClick', index)
			}
		}
	}
</script>

<style scoped>
	.tab-control {
		display: flex;
		text-align: center;
		font-size: 15px;
		height: 40px;
		line-height: 40px;
	}
	.tab-control-item {
		flex: 1;
	}
	span {
		padding: 3px 5px;
	}
	.active {
		color: #ff5777;
	}
	.active span{
		border-bottom: 3px solid #ff5777;
	}
	
</style>
