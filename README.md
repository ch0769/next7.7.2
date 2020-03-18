部署上传
Deployment: hexo g -d
本地调试
hexo clean && hexo g && hexo s

官方教程 https://theme-next.org/docs/theme-settings/posts#wordcount-2
发布字数统计
npm install hexo-symbols-count-time
网站加入
symbols_count_time:
  symbols: true
  time: true
  total_symbols: true
  total_time: true
主题加入
symbols_count_time:
  separated_meta: true
  item_text_post: true
  item_text_total: true
  awl: 4
  wpm: 275

统计与分析
Busuanzi

评论 Valine

本地搜寻
npm install hexo-generator-searchdb
主题设置
local_search:
  enable: true


主题美化
https://theme-next.org/docs/third-party-services/external-libraries#Backgroud-JS

修改主题下 _config.yml 文件，搜索 ustom_file_path:
 最后一个去掉#号
style: source/_data/styles.styl

your_blog/source/_data/styles.styl，注意是博客根目录下的 source/ 而不是主题下的目录 source/，
然后我们就可以在这个文件里边添加自定义配置。

移动设备适应
mobile_layout_economy: true

页脚
网站开始时间
footer:
  since: 2015

网站版权名称
footer:
  copyright:

备案
footer:
  beian:
    enable: true
    icp: 京ICP备 1234567890号-1
    gongan_id: 1234567890
    gongan_num: 京公网安备 1234567890号
    gongan_icon_url: /uploads/beian.png

侧边

侧边栏网站状态

site_state: true

侧边社交链接
social

可加 RSS: /atom.xml || rss

网站链接
links:
  Title1: http://example1.com/
  Title2: http://example2.com/
回到顶部
back2top:
  enable: true

相关热门贴
related_posts:
  enable: ture

捐赠
reward_settings:
  # If true, reward would be displayed in every article by default.
  # You can show or hide reward in a specific article throuth `reward: true | false` in Front-matter.
  enable: true
  animation: false
  #comment: Donate comment here

reward:
  wechatpay: /images/wechatpay.png
  alipay: /images/alipay.png
  bitcoin: /images/bitcoin.png




自定义徽标支持
next/_config.yml

custom_logo: /uploads/custom-logo.jpg




阅读进度

reading_progress:
  enable: true
  color: "#37c6c0"
  height: 2px

书签

bookmark:
  enable: true
  # Customize the color of the bookmark.
  color: "#222"
  # If auto, save the reading progress when closing the page or clicking the bookmark-icon.
  # If manual, only save it by clicking the bookmark-icon.
  save: auto

GitHub横幅

github_banner:
  enable: true
  permalink: https://github.com/yourname
  title: Follow me on GitHub


自定义页面
cd your-hexo-site
 hexo new page custom_name    #创建一个新的custom_name页面

添加«标签»页面
 cd your-hexo-site
 hexo new page tags

