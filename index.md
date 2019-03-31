## 简介

  欢迎来到小猪猪的开放API!
  
  本API特性:
  1. 承诺开放API永久免费，同时每月提供10GB流量供您使用。
  2. 无需注册，无需key，随时随地想用就用!
  3. 保证持续更新，有问题请及时反馈给我们!
  
  注意:接口暂不支持Https，请耐心等待开发......

## 百度免费图片CDN加速 API
  
  API地址:`http://api.ypig.tk/picturecdnapi.php`
  
  名称|必须|示例
  --|:--:|--:
  url|是|[https://s2.ax1x.com/2019/03/31/Arr1rq.jpg](https://s2.ax1x.com/2019/03/31/Arr1rq.jpg)
  
  返回结果
  ```
  https://graph.baidu.com/resource/10652ec7155abf116673401554033653.jpg
  ```
  
  备注:该功能不是图床，仅提供CDN加速服务。
  
## 手机号归属地查询 API
  
  API地址:`http://api.ypig.tk/mobilesegmentapi.php`
  
  名称|必须|示例
  --|:--:|--:
  telephone|是|18888888888
  
  返回结果
  ```
  {
    mts: '1888888',
    province: '北京',
    catName: '中国移动',
    telString: '18888888888',
    areaVid: '29400',
    ispVid: '3236139',
    carrier: '北京移动'
  }
  ```
  
## 天气预报 API
  
  API地址:`http://api.ypig.tk/weatherapi.php`
  
  名称|必须|示例
  --|:--:|--:
  province|是|北京
  city|是|北京
  
  
  返回结果
  ```
  {
    "data": {
      "alarm": {},
      "forecast_1h": {
        "0": {
          "degree": "12",
          "update_time": "20190331190000",
          "weather": "多云",
          "weather_code": "01",
          "weather_short": "多云",
          "wind_direction": "南风",
          "wind_power": "3"
        },
        "1": {
          "degree": "10",
          "update_time": "20190331200000",
          "weather": "多云",
          "weather_code": "01",
          "weather_short": "多云",
          "wind_direction": "西北风",
          "wind_power": "3"
        },
        ......
      },
      "forecast_24h": {
        "0": {
          "day_weather": "晴",
          "day_weather_code": "00",
          "day_weather_short": "晴",
          "day_wind_direction": "北风",
          "day_wind_direction_code": "8",
          "day_wind_power": "5",
          ......
        },
        ......
      },
      "index": {
        "airconditioner": {
          "detail": "您将感到很舒适，一般不需要开启空调。",
          "info": "较少开启",
          "name": "空调开启"
        },
        "allergy": {
          "detail": "天气条件易诱发过敏，易过敏人群应减少外出，外出宜穿长衣长裤并佩戴好眼镜和口罩，外出归来时及时清洁手和口鼻。",
          "info": "易发",
          "name": "过敏"
        },
        "carwash": {
          "detail": "较适宜洗车，未来一天无雨，风力较小，擦洗一新的汽车至少能保持一天。",
          "info": "较适宜",
          "name": "洗车"
        },
        ......
      "limit": {
        "tail_number": "不限行",
        "time": "20190331"
      },
      "tips": {
        "observe": {
          "0": "光芒透过云缝，洒向大地~",
          "1": "现在的温度比较凉爽~"
        }
      }
    },
    "message": "OK",
    "status": 200
  }
  ```

## 短链接生成 API
  
  API地址:`http://api.ypig.tk/shortlinkapi.php`
  
  名称|必须|示例
  --|:--:|--:
  url|是|[https://ypig.tk/](https://ypig.tk/)
  
  返回结果
  ```
  {
    "url_short": "http://t.cn/EciWLK7",
    "url_long": "https://ypig.tk/",
    "type": 0
  }
  ```
  
## 腾讯游戏新闻 API
  
  API地址:`http://api.ypig.tk/gamenewsapi.php`
  
  本API无需携带参数请求
  
  返回结果
  ```
  {
    "code": 0,
    "msg": "index",
    "data": [{
      "app_id": "20190331A0E97900",
      "article_type": 1,
      "bimg": "https://inews.gtimg.com/newsapp_bt/0/7047949212/641",
      "category": "games",
      "category1_chn": "游戏",
      "category1_id": "10",
      "category2_chn": "王者荣耀",
      "category2_id": "1024",
      "category_chn": "游戏",
      "category_id": "10",
      "comment_id": "3817198725",
      "comment_num": 0,
      "duration": 0,
      "ext": {
        "tonality_score": 0,
        "news_score": 3,
        "img_type": 3,
        "video_count": 0
      },
      "flag": 0,
      "fm_url": "",
      "from": "kuaibao",
      "id": "20190331A0E979",
      "img": "https://inews.gtimg.com/newsapp_bt/0/7047949212/641",
      "img_count": 5,
      "img_type": 3,
      "imgs": {
        "295X195": "https://inews.gtimg.com/newsapp_ls/0/8372904247_294195/0",
        "354X264": "https://inews.gtimg.com/newsapp_ls/0/8372904247_354264/0"
      },
      "intro": "王者荣耀中若是只能使用一技能，最强的英雄是哪位？90％都选她",
      "irs_imgs": {
        "295X195": ["https://inews.gtimg.com/newsapp_ls/0/8372904247_294195/0", "https://inews.gtimg.com/newsapp_ls/0/8372904249_294195/0", "https://inews.gtimg.com/newsapp_ls/0/8372983493_294195/0"],
        "354X264": ["https://inews.gtimg.com/newsapp_ls/0/8372904247_354264/0", "https://inews.gtimg.com/newsapp_ls/0/8372904249_354264/0", "https://inews.gtimg.com/newsapp_ls/0/8372983493_354264/0"]
      },
      "keywords": "王者荣耀;王者荣耀\u0026吕布;王者荣耀\u0026伽罗",
      "media_icon": "https://inews.gtimg.com/newsapp_ls/0/4349689985_200200/0",
      "mini_img": "",
      "multi_imgs": ["https://inews.gtimg.com/newsapp_bt/0/7047949212/641", "https://inews.gtimg.com/newsapp_bt/0/3220253088/641", "https://inews.gtimg.com/newsapp_bt/0/2517381499/641"],
      "news_level": 3,
      "play_url_high": "",
      "play_url_medium": "",
      "play_url_small": "",
      "pool_type": "irs:img",
      "publish_time": "2019-03-31 20:12:22",
      "report": "{\"ext\": \"0+0\"+ \"all\": \";;;0+0\"+ \"3h\": \"43441+7861;39+448;games:0+0;0+0\"+ \"day\": \"275162+46533;442+2411;games:0+0;0+0\"}",
      "s_group": 0,
      "source": "悟空讲王者",
      "source_fans": 0,
      "source_id": "10605364",
      "source_logo": "",
      "strategy": 2,
      "surl": "http://kuaibao.qq.com/s/20190331A0E97900",
      "tag_label": [
        ["王者荣耀", "204791"],
        ["王者荣耀\u0026吕布", "296854"],
        ["王者荣耀\u0026伽罗", "147814579"]
      ],
      "tags": "王者荣耀;王者荣耀\u0026吕布;王者荣耀\u0026伽罗",
      "title": "王者荣耀中若是只能使用一技能，最强的英雄是哪位？90％都选她",
      "ts": 1554034342,
      "update_time": "2019-03-31 20:12:22",
      "url": "https://xw.qq.com/cmsid/20190331A0E97900",
      "view_count": 0,
      "vurl": "https://new.qq.com/omn/20190331/20190331A0E97900"
       ...
    }],
    "datanum": 7,
    "seq": "20190331202045-rpPL4ggWnSNwLd4X",
    "biz": 5999,
    "s_group": "0",
    "other": null
  }
  ```
  
  >以下为私有接口，仅提供给合作个人使用，不对外开放。

## 新加坡加速 API
  
  **注意:本API地址已经迁移到专有页面**
  API地址:`http://ssr.ypig.tk/ssrapi.php`
  
  名称|必须|示例
  --|:--:|--:
  token|是|TOKEN
  
  返回结果
  ```
  ssr://test
  ```
  
## 节点测速 API
  
  **注意:本API地址已经迁移到专有页面**
  API地址:`http://ssr.ypig.tk/pingapi.php`
  
  名称|必须|示例
  --|:--:|--:
  node|是|test
  
  返回结果
  ```
  0.50000
  ```

  ---
  以上就是全部API接口，更多接口正在持续更新中，欢迎访问[黄猪官网](https://ypig.tk/)探索更多有趣的小工具!
