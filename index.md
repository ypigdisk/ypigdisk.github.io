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
  
  API地址:`http://api.ypig.tk/phonesegment.php`
  
  名称|必须|示例
  --|:--:|--:
  telephone|是|18888888888
  
  返回结果
  ```
  https://graph.baidu.com/resource/10652ec7155abf116673401554033653.jpg
  ```
  
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
