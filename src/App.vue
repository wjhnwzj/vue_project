<template>
    <div class="app-container">
      <!-- 顶部 header区域 -->
      <mt-header fixed title="Vue项目"></mt-header>
      <!-- 中间的 路由 router-view 区域 -->
		<transition mode="out-in">
		<router-view></router-view>
		</transition>

      <!-- 底部 Tabbar 区域 -->
      <nav class="mui-bar mui-bar-tab">
			<router-link class="mui-tab-item " to="/home">
				<span class="mui-icon mui-icon-home"></span>
				<span class="mui-tab-label">首页</span>
			</router-link>
			<router-link class="mui-tab-item" to="/member">
				<span class="mui-icon mui-icon-contact"></span>
				<span class="mui-tab-label">会员</span>
			</router-link>
			<router-link class="mui-tab-item" to="/shopcart">
				<span class="mui-icon mui-icon-extra mui-icon-extra-cart"><span class="mui-badge">0</span></span>
				<span class="mui-tab-label">购物车</span>
			</router-link>
			<router-link class="mui-tab-item" to="/search">
				<span class="mui-icon mui-icon-search"></span>
				<span class="mui-tab-label">搜索</span>
			</router-link>
		</nav>
    </div>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.app-container{
  padding-top: 40px
}

.v-enter,.v-leave-to{
	opacity: 0;
	transform: translateX(150px)
}

.v-enter-active,.v-leave-active{
	transition: all 0.3s ease
}
</style>
