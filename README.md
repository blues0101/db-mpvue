# db-films

> A Mpvue project

## Build Setup

``` bash
# 初始化项目
vue init mpvue/mpvue-quickstart myproject
cd myproject

# 安装依赖
yarn

# 开发时构建
npm dev

# 打包构建
npm build

# 指定平台的开发时构建(微信、百度、头条、支付宝)
npm dev:wx
npm dev:swan
npm dev:tt
npm dev:my

# 指定平台的打包构建
npm build:wx
npm build:swan
npm build:tt
npm build:my

# 生成 bundle 分析报告
npm run build --report

# 因豆瓣接口时常变动,数据是本地写死的(详情页是调用接口)，目前把线上调用api贴出来，方便查阅！！！
获取正在热映的电影：https://douban.uieee.com/v2/movie/in_theaters
访问参数：
start : 数据的开始项
 
count：单页条数
 
city：城市
 
获取电影Top250：https://douban.uieee.com/v2/movie/top250
访问参数：
start : 数据的开始项
 
count：单页条数
 
获取即将上映电影：https://douban.uieee.com/v2/movie/coming_soon
访问参数：
start : 数据的开始项
 
count：单页条数
 
电影搜索：https://douban.uieee.com/v2/movie/search
访问参数：
start : 数据的开始项
 
count：单页条数
 
q：要搜索的电影关键字
 
tag：要搜索的电影的标签
 
电影详情：https://douban.uieee.com/v2/movie/subject/:id
访问参数：电影id
如：电影《小飞象》的电影id为：25924056，搜索此电影的详细信息：
https://api.douban.com/v2/movie/subject/25924056
 
电影本周口碑榜： https://douban.uieee.com/v2/movie/weekly?apikey=0df993c66c0c636e29ecbb5344252a4a
北美票房榜： https://douban.uieee.com/v2/movie/us_box?apikey=0df993c66c0c636e29ecbb5344252a4a
新片榜： https://douban.uieee.com/v2/movie/new_movies?apikey=0df993c66c0c636e29ecbb5344252a4a
影人剧照: https://douban.uieee.com/v2/movie/celebrity/:id/photos?apikey=0df993c66c0c636e29ecbb5344252a4a
电影条目剧照： https://douban.uieee.com/v2/movie/subject/:id/photos?apikey=0df993c66c0c636e29ecbb5344252a4a
豆瓣音乐
搜索 https://douban.uieee.com/v2/music/search?q=欧美&count=15?
详情 https://douban.uieee.com/v2/music/:id
豆瓣图书
搜索，例如：
https://douban.uieee.com/v2/book/search?q=虚构类&count=8 
https://douban.uieee.com/v2/book/search?q=非虚构类&count=8 
https://douban.uieee.com/v2/book/search?q=旅行&count=8
获取电影条目短评论: https://douban.uieee.com/v2/movie/subject/:id/comments?start=xxx&count=xxx&apikey=0df993c66c0c636e29ecbb5344252a4a
```
