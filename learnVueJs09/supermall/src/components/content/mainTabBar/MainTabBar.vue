<template>
	<tab-bar>
		<tab-bar-item path="/home" activeColor="#31c6ce">
			<img slot="item-icon" src="~assets/img/tabbar/ico_home_tabbar_nor.png" alt="">
			<img slot="item-icon-active" src="~assets/img/tabbar/ico_home_tabbar_sel.png" alt="">
			<div slot="item-text">首页</div>
		</tab-bar-item>
		<tab-bar-item path="/category" activeColor="#31c6ce">
			<img slot="item-icon" src="~assets/img/tabbar/ico_list_tabbar_nor.png" alt="">
			<img slot="item-icon-active" src="~assets/img/tabbar/ico_list_tabbar_sel.png" alt="">
			<div slot="item-text">分类</div>
		</tab-bar-item>
		<tab-bar-item path="/cart" activeColor="#31c6ce">
			<img slot="item-icon" src="~assets/img/tabbar/ico_product_tabbar_nor.png" alt="">
			<img slot="item-icon-active" src="~assets/img/tabbar/ico_product_tabbar_sel.png" alt="">
			<div slot="item-text">购物车</div>
		</tab-bar-item>
		<tab-bar-item path="/profile" activeColor="#31c6ce">
			<img slot="item-icon" src="~assets/img/tabbar/ico_my_tabbar_nor.png" alt="">
			<img slot="item-icon-active" src="~assets/img/tabbar/ico_my_tabbar_sel.png" alt="">
			<div slot="item-text">我的</div>
		</tab-bar-item>
	</tab-bar>
</template>

<script>
	import TabBar from 'components/common/tabbar/TabBar'
	import TabBarItem from 'components/common/tabbar/TabBarItem'

	export default {
		name: 'MainTabBar',
		components: {
			TabBar,
			TabBarItem
		}
	}
</script>

<style>
</style>
