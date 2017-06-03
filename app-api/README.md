# yorkba-doc

# app接口使用说明



## 1.系统参数定义

|参数名称|参数含义|
|---|---|
|app_id|渠道号|
|nonce|随机数|
|timestamp|时间戳|
|version|版本号|
|build|构建号|
|udid|设备唯一标识：android对应imei，ios对应idfa|
|devicemodel|设备类型|
|sysname|系统名称|
|sysversion|系统版本|
|sign|签值|


## 2.加签规则

 调用接口时需要传系统参数和业务参数：
 
> 1.将请求参数（不包括sign和资源文件）按照keyname快速排序

> 2.将排序后的参数使用&符号，依照key=value的形式连接成字符串

> 3.计算拼接后字符串的MD5值
 
 
## 3.服务器

 
