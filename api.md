移动API的开发文档
==================

关于API文档开发过程

### 个人首页API

  Class: ApiUserController
  
  Function: index
  
  URL: 'api/people/{id}', id为整数型，为用户的id值。
  
  Method: GET
  
  Return: 返回一个自己个人资料，发布的所有视频，还有视频的评论。
  
### 个人评论消息API
  Class: ApiUserController
  
  Function: messages
  
  URL：'api/people/{id}/message', id为整数型，用户的id值，
  
  Method: GET
  
  Return: 返回其他用户或是系统对自己的评论（或消息）。
  
### 个人资料API
  
  Class: ApiUserController
  
  Function: postProfile
  
  URL: 'api/profile/{id}', id为整数型，为个人资料的id值，不是用户id,这个用户资料的id值可以在个人首页API中获得

  Method: POST
  
  Input: [个人资料的字段](https://github.com/wingeek/miao-docs/blob/master/models/profile.md)。
  
  Return: error or success message ??
  
### 个人头像上传API

  Class: ApiUserController
  
  Function: uploadAvatar
  
  Input: image source data原始图像数据
  
  URL: 'api/avatar/{id}', id为用户的id值。
  
  Method: POST
  
  Return: 返回成功： url for ios image size
          返回失败： 必要的信息和[错误代码](https://github.com/wingeek/miao-docs/edit/master/errorcodes.md).
         
  说明： 图片自动切割为20x20, 100x100, 210x210三种尺寸 

### 应用首页API


### 用户个人资料编辑API

