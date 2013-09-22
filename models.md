数据模型
==========

关于数据模型的开发文档

### 微电影模型

  微电影是短视频的结合产物，建立独立的Film和films数据表对微电影进行数据管理。
  
  模型名: Film
  
  数据表：films
  
  属性：id, title, description, filepath, format, topic_id, user_id, votes, browses, thumbnail
  
  关系：
  
    one- many: 
    
    many- one: Topic, User

