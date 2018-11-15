# 产品功能

在您使用对象存储产品之前，建议您先阅读对象存储相关的基础概念，这里详细介绍了Bucket、Object的创建命名规则以及Region、Endpoint、AccessKey等定义，这些可以帮助您更好地理解以下功能介绍和描述。

对象存储提供以下功能：

|功能|描述|
|-|-|
|创建存储空间|在上传任何文件到 OSS 之前，您需要首先创建存储空间来存储文件。|
|删除存储空间|如果您不再需要存储空间，请将其删除以免进一步产生费用。|
|修改存储空间读写权限| OSS 提供权限控制Bucket Policy，在创建存储空间的时候选择相应的权限控制，也可以在创建之后，在权限设置中修改 Bucket Policy。|
|设置防盗链|为了减少您存储于 OSS 的数据被其他人盗链而产生额外费用，OSS 支持设置基于 HTTP header 中表头字段 referer 的防盗链方法。|
|跨域访问设置|OSS 提供 HTML5 协议中的跨域资源共享 CORS 设置，帮助您实现跨域访问。|
|静态网站托管|您将图片、视频、静态页面等资源上传到OSS的Bucket后，可以为该空间指定默认首页、错误返回页及访问发生错误后的重定向地址。通过该功能，用户就可以将某个Bucket作为一个静态网站来使用。|
|跨区域复制|跨区域复制是对不同区域的存储空间中的文件进行自动异步复制。它将源存储空间的文件的改动（除删除操作）从源存储空间复制到不同区域的目标存储空间。|
|上传文件|您可以上传任意类型文件到存储空间中。|
|新建文件夹|您可以像管理 Windows 文件夹一样管理 OSS 文件夹。|
|搜索文件|在存储空间或文件夹中搜索具有相同的名称前缀的文件。|
|获取文件外链|通过获取已上传文件的外链访问地址进行文件的分享和下载。|
|删除文件|删除单个文件。|
|删除文件夹|删除单个文件夹。|
|用量监控|了解OSS服务的使用情况，包括相关数据和用量监控图表。|
|图片服务|对保存在OSS上的图片进行格式转换、剪裁、缩放、旋转、水印、样式封装等各种处理。|
|视频服务|提供多种视频格式的转码服务。|
|API|提供 OSS支持的 RESTful API 操作和相关示例。|
|SDK|提供主流语言 SDK 的开发操作和相关示例。|