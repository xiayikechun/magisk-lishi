# Magisk自定义更新源
## 获取下载源
历史版本Magisk自定义更新源：
https://www.mintimate.cn/2020/03/08/Magisk

## Blog
更多内容，欢迎访问：
[Mintimate's Blog 只为与你分享](https://www.mintimate.cn)

# 如何自己做源？
Magisk的更新源，其实就是一段Json数据：
{
  "app": {
    "version": "",
    "versionCode": "",
    "link": "",
    "note": ""
  },
  "uninstaller": {
    "link": ""
  },
  "magisk": {
    "version": "",
    "versionCode": "",
    "link": "",
    "md5": ""
  },
  "message":{
  	"Power By":"",
  	"Address":""
  }
}
其中，对象app、magisk为必须。

# 联系我
如果想捐赠或者联系我，可以访问博客关于页面：
[Mintimate's Blog 关于页面](https://mintimate.cn/about/)