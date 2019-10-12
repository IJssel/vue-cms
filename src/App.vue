<template>
  <div class="app-container">

    <!-- 中间的 路由 router-view 区域 -->
		<transition>
			<router-view></router-view>
		</transition>


    <router-view />




    <!-- 底部 Tabbar 区域 -->
    <!-- <nav class="mui-bar mui-bar-tab">
			<router-link class="mui-tab-item-llb" to="/home">
				<span class="mui-icon iconfont icon-biaodan"></span>
				<span class="mui-tab-label">生活</span>
			</router-link>
			<router-link class="mui-tab-item-llb" to="/member">
				<span class="mui-icon iconfont icon-gouwudai"></span>
				<span class="mui-tab-label">商城</span>
			</router-link>
			<router-link class="mui-tab-item-llb" to="/shopcar">
				<span class="mui-icon iconfont icon-aixin">
					<span class="mui-badge" id="badge">{{ $store.getters.getAllCount }}</span>
				</span>
				<span class="mui-tab-label">助手</span>
			</router-link>
			<router-link class="mui-tab-item-llb" to="/search">
				<span class="mui-icon iconfont icon-faxian"></span>
				<span class="mui-tab-label">发现</span>
			</router-link>
      <router-link class="mui-tab-item-llb" to="/search">
				<span class="mui-icon mui-icon-person"></span>
				<span class="mui-tab-label">我的</span>
			</router-link>
		</nav> -->

    <van-tabbar route class="mui-bar-tab">
      <van-tabbar-item replace to="/home" icon="wap-home-o">首页</van-tabbar-item>
      <van-tabbar-item replace to="/member" icon="friends-o">社区</van-tabbar-item>
      <van-tabbar-item replace to="/shopcar" icon="comment-o">消息</van-tabbar-item>
      <van-tabbar-item replace to="/shopcar" icon="shopping-cart-o">购物车</van-tabbar-item>
      <van-tabbar-item replace to="/search" icon="contact">我的</van-tabbar-item>
    </van-tabbar>

  </div>
</template>

<script>
// export default {
//   data() {
//     return {
//       flag: false
//     };
//   },
//   created() {
//     this.flag = this.$route.path === "/home" ? false : true;
//   },
//   methods: {
//     goBack() {
//       // 点击后退
//       this.$router.go(-1);
//     }
//   },
//   watch: {
//     "$route.path": function(newVal) {
//       if (newVal === "/home") {
//         this.flag = false;
//       } else {
//         this.flag = true;
//       }
//     }
//   }
// };
</script>




// <style lang="scss" scoped>
// .mint-header {
//   z-index: 99;
// }
// .app-container {
//   padding-top: 40px;
//   padding-bottom: 50px;
//   overflow-x: hidden;
// }

// .v-enter {
//   opacity: 0;
//   transform: translateX(100%);
// }

// .v-leave-to {
//   opacity: 0;
//   transform: translateX(-100%);
//   position: absolute;
// }

// .v-enter-active,
// .v-leave-active {
//   transition: all 0.5s ease;
// }

// // 该类名，解决 tabbar 点击无法切换的问题
// .mui-bar-tab  {
//   color: #f2f2f2;
// }
// .mui-tab-item-llb.mui-active {
//   color: #e3657a;
// }

// .mui-bar-tab .mui-tab-item-llb {
//   display: table-cell;
//   overflow: hidden;
//   width: 1%;
//   height: 80px;
//   text-align: center;
//   vertical-align: middle;
//   white-space: nowrap;
//   text-overflow: ellipsis;
//   color: black;
// }

// .mui-bar-tab .mui-tab-item-llb .mui-icon {
//   top: 3px;
//   width: 25px;
//   height: 25px;
//   padding-top: 0;
//   padding-bottom: 0;
// }

// .mui-bar-tab .mui-tab-item-llb .mui-icon ~ .mui-tab-label {
//   font-size: 13px;
//   display: block;
//   overflow: hidden;
//   text-overflow: ellipsis;
// }
// </style>
