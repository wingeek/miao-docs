### 视频评论模型

  	$table->increments('id');
	$table->integer('user_id');
	$table->integer('video_id');
	$table->integer('commenter_id');
	$table->integer('reply_id')->default(0);
	$table->text('body');
	$table->timestamps();
	
	user_id: video creater's id
	
	video_id: video's id
	
	commenter_id: 评论者的id
	
	reply_id: 如果评论是给评论的回复，那么就是那条评论的commenter_id值,默认值为0
	
	body: comment content
	
	
	
	
	
