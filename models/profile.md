## 个人资料模型

  	$table->increments('id');
	$table->integer('user_id');
	$table->date('birthday');
	$table->boolean('male');
	$table->text('description');
	$table->string('hobby');
	$table->string('telephone')->after('user_id');
    $table->string('constellation')->after('telephone');
    $table->string('qq')->after('constellation');
    $table->string('douban')->after('qq');
    $table->string('weibo')->after('douban');
    $table->string('site')->after('weibo');
    $table->string('address')->after('site');
    $table->string('prefession')->after('address');
    $table->string('bloodtype',6)->after('prefession');
	$table->timestamps();
