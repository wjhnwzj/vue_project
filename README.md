#这是一个用Vue+MUI+mint-ui开发的项目

##制作首页APP组件
1.完成Header区域，使用的是 Mint-UI 中的Header组件
2.制作底部的Tabbar区域，使用的是MUI的Tabbar.html
+在制作 购物车小图标的时候，操作会相对多一些
+先把扩展图标的css样式，复制到项目中
+复制扩展字体库ttf文件，到项目中
+为购物车小图标，添加如下样式 mui-icon-extra mui-icon-extra-cart
3.要在中间区域放置一个router-view展示路由匹配到的组件

##改造tabbar 为 router-link

##设置路由高亮
将路由中的linkActiveClass高亮属性的值改为'mui-active',默认的值为'router-link-active'

##点击tabbar中的路由链接，展示对应的路由组件

##制作首页轮播图布局(在Home组件中显示轮播图)

##加载首页轮播图数据
1.获取数据，使用 vue-resource
