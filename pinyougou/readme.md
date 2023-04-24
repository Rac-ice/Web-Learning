# 电商平台

## 目录文件夹

| 名称 | 说明 |
| --- | --- |
| 项目文件夹 | pinyougou |
| 样式类图片文件夹 | img |
| 样式文件夹 | css |
| 产品类图片文件夹 | upload |
| 字体类文件夹 | fonts |
| 脚本文件夹 | js |

## 样式文件的分类

- 初始化css（css reset）让浏览器风格统一，把常用的初始化语句放入base.css里
- 把一些公共的样式放入common.css里

## 首页布局

| 名称 | 说明 |
| --- | --- |
| 快捷导航栏 | shortcut |
| 头部 | header |
| 标志 | logo |
| 购物车 | shopcar |
| 搜索 | search |
| 热点词 | hotwords |
| 导航 | nav |
| 导航左侧 | dropdown 包含 .dd .dt |
| 导航右侧 | navitems |

### 1).shortcut制作

- 通栏的盒子 命名为shortcut 快捷导航栏的意思，给个行高，可以继承给里面的子盒子
- 里面包含 版心的盒子
- 版心盒子里面包含1号左侧盒子左浮动
- 版心盒子里面包含2号右侧盒子右浮动

### 2).header制作

- header盒子必须要有高度
- 1号盒子是logo标志 定位
- 2号盒子是 search 搜索模块 定位
- 3号盒子 hotwords 热词模块 定位
- 4号盒子 shopcar 购物车模块
1.count 统计部份 用绝对定位
2.count 统计部份 不要给宽度 让件数撑开 给一个高度
3.左下角不是圆角 其余三个是圆角

### 3).nav 制作

- nav 盒子通栏有高度 而且有个下边框
- 1号盒子 左侧浮动 dropdown 下拉导航 里面包含 dt dd
- 2号盒子 右侧浮动 navitems 导航栏组

### 4).footer 制作

- footer 页面底部盒子 通栏 给一个高度 灰色背景
- footer 里面 一个版心
- 版心里面包含 1号盒子 mod_service 服务模块 module 模块的意思
- 版心里面包含 2号盒子 mod_help 帮助模块
- 版心里面包含 3号盒子 mod_copyright 版权模块

### 5).main 主体模块制作

- main 盒子 宽度 980px 距离 左边 220 给个margin-left 给高度不用清除浮动
- main 里面包含 左侧盒子 左浮动 focus 焦点图模块
- main 里面包含 右侧盒子 右浮动 newsflash 新闻快报模块

### 6).newsflash 新闻快报模块制作

- 1 号盒子 为 news 新闻模块
- 2 号盒子 为 lifeservice 生活服务模块
- 3 号盒子 为 bargain 特价商品模块

### 7).news 新闻模块制作

- 分为 上下两个模块 都用div
- 1 号盒子 news-hd 新闻头部模块 给一个 高度 和 下边框
- 2 号盒子 news-bd 新闻主题部分 里面 包含 ul 和 li 以及 a

### 8).lifeservice 生活服务模块制作

- lifeservice 盒子 宽度为 250 装不下4个li
- 让 lifeservice 里面 ul 宽度为 252 可以装下4个li
- lifeservice 盒子 overflow 隐藏多余部分

### 9).**recommend 推荐模块制作**

- 里面包含2个盒子， 浮动即可
- 1 号盒子 recom-hd
- 2 号盒子 recom-bd 小 竖线

### 10).**floor 楼层区**

floor 一个大盒子 包含 不给高度 内容有多少 算多少

### 11).**家用电器模块**

- jiaju 不给高度 内容撑开 要清除浮动
- 版心居中对齐
- 1 号盒子 box-hd 给一个高度 有下边框 里面分为左右2个盒子
- 2 号盒子 box-bd 不给高度

### 12).box-hd 模块

- 有高度
- 左边 h3 盒子
- 右边 div 命名 tab-list 用到 tab切换效果 里面用 ul 和 li

### 13).侧边栏 fixedtool

固定定位 里面包含 li

## 列表页布局

- 列表页 头部 和 底部 基本一致
- 复制粘贴 头部 和 底部
- 引入相关样式

### 1).列表页 header nav 修改

- 盒子 sk 定位 second kill
- 1 号盒子 左侧浮动 sk_list 里面包含 ul 和 li
- 2 号盒子 右侧浮动 sk_con 里面包含 ul 和 li

### 2).列表页 主体盒子 sk_container

里面包含 所有的 列表页的所有主体内容

- 1 号盒子 sk_container 给宽度 1200 不给高度
- 2 号盒子 sk_hd 插入图片
- 3 号盒子 sk_bd 里面包含 ul 和 li

### 3).sk_goods 布局

- 1 号位置 有 a 包含 图片 和 标题 插入图片 sk_goods_img 鼠标放入图片 上滑动效果
- 2 号位置 标题 h5 命名 sk_goods_title
- 3 号位置 价格 div 命名 sk_goods_price
- 4 号位置 div  命名 sk_goods_progress 导航条
- 5 号位置 a 命名 sk_goods_buy 使用定位

### 4).分页制作 page

- 通栏盒子 div 命名 page 里面全部 行内块
- 1 号盒子 span 命名 page_num 页码 里面放 a a转换为行内块
pg_prev 上一页 pg_next 下一页
- 2 号盒子 span 命名 page_skip 跳转 里面 input 和 button

## 详情页布局

| 名称 | 说明 |
| --- | --- |
| 主体 | de_container |
| 面包屑导航 | crumb_wrap |
| 产品介绍 | product_intro （ introduction介绍） |
| 预览包 | preview_wrap（左侧部分） |
| 预览缩略图 | preview_img |
| 预览列表 | preview_list |
| 左按钮 | arrow_prev |
| 右按钮 | arrow_next |
| 小图列表 | preview_items |
| 产品详细信息区域 | itemInfo_wrap（右侧部分） |
| 头部名称 | sku_name （skull 头骨） |
| 新闻 | news |
| 摘要 | summary |
| 评价 | remark |
| 价格摘要 | summary_price |
| 配送至 | summary_stock |
| 支持 | summary_support |
| 选择 | choose |
| 选择按钮组 | choose_btns |
| 选择数量 | choose_amount |
| 减去 | reduce |
| 加入购物车 | addshopcar |
| 产品细节 | product_detail （detail描述） |
| 左侧边 | aside |
| 详细描述 | detail |

### 1).**面包屑导航**

- crumb_wrap 面包屑导航

### 2).**产品介绍 模块**

- 1 号盒子 命名 product_intro （ introduction介绍） 产品模块 不给高度 左右两个盒子
- 2 号盒子 预览区域 preview_wrap 给宽度 给高度 左浮动
- 3 号盒子 产品详细信息区域 itemInfo_wrap 给宽度 不给高度 右浮动

### 3).预览区域制作

- 1 号盒子 图片预览 命名 preview_img
- 2 号盒子 预览列表 命名 preview_list

### 4).**preview_list 制作**

- 盒子 有左右按钮 arrow_prev arrow_next 定位
- 中间 用 ul 命名 list-item 给宽度和高度  margin: 0 auto; 水平居中对齐

### 5).**产品详细信息区域制作 itemInfo_wrap**

- 1 号盒子 为 头部 sku_name
- 2 号盒子 为 最新新闻 news
- 3 号盒子 为 产品详细摘要 命名 summary

| 名称 | 说明 |
| --- | --- |
| 头部名称 | sku_name |
| 新闻 | news |
| 摘要 | summary |
| 评价 | remark |
| 价格摘要 | summary_price |
| 促销摘要 | summary_promotion |
| 配送至 | summary_stock |
| 支持 | summary_support |
| 选择 | choose |
| 选择版本 | choose_version |
| 选择类型 | choose_type |
| 选择按钮组 | choose_btns |
| 选择数量 | choose_amount |
| 减去 | reduce |
| 加入购物车 | addshopcar |

### 6).**产品细节模块 product_detail**

- 大盒子 product_detail 不给高度 清除浮动
- 1 号盒子 左侧浮动 命名 aside 有宽度 不给高度
- 2 号盒子 右侧浮动 命名 detail 有宽度 不给高度

### 7).**aside 布局**

- 1 号盒子 命名 tab_list 给高度 里面 ul 和 li
- 2 号盒子 命名 tab_con 里面多个 ul item 和 tab_list里的li 一一对应

### 8).**detail 布局**

- 1 号盒子 命名 detail_tab_list 给高度 里面 ul 和 li
- 2 号盒子 命名 detail_tab_con 里面多个 ul item 和 tab_list里的li 一一对应

## **注册页面**

| 名称 | 说明 |
| --- | --- |
| 注册专区 | registerarea |
| 注册内容 | reg-form |
| 错误的 | error |
| 成功的 | success |
| 默认的 | default |