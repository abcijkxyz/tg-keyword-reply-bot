# telegram 关键词自动回复机器人 开源版本
telegram 关键词回复机器人，群主助手



### 命令介绍
- 添加关键词回复规则 `/add 关键词===回复内容` 或者 `/add 关键词1||关键词2===回复内容` 
- 关键词可以使用正则表达式,例如`/add re:p([a-z]+)ch===测试正则`,就会匹配规则`p([a-z]+)ch`  
- 删除关键词规则 `/del 关键词` 暂不支持一次性删除多个关键词
- 自动删除含有关键词的文字消息, 只需要将回复内容设置成 `delete`, 并给机器人添加删除消息权限
- 使用`/list`命令可以查看本群内所有自动回复规则
- 给机器人添加删除消息和踢人的管理权限,可以自动防清真(阿拉伯语)

### 回复特殊内容
- 回复内容支持文字\图片\GIF\视频,默认文字
- 如需图片,回复内容设置成`photo:https://t.me/c/1472018167/53095`,`https://t.me/c/1472018167/53095`是已经发送过的图片获取到的链接
- 同理,gif将`photo`替换成`gif`,视频替换成`video`,文件替换成`file`
- 注意: 这里的链接必须是公开群组的,否则无法发出来


### 后续增加功能的使用说明见： 
##### [使用说明](https://telegra.ph/%E8%BF%99%E4%B8%AA%E6%88%91%E7%9F%A5%E9%81%93%E6%9C%BA%E5%99%A8%E4%BA%BA%E4%BD%BF%E7%94%A8%E8%AF%B4%E6%98%8E-07-07)


## 使用最新版本可执行文件搭建
旧版本代码开源，新版本代码不再开源，但是随时更新新版本的可执行文件      
进入 [Release 页面](https://github.com/zu1k/tg-keyword-reply-bot/releases) 下载最新版本可执行文件到服务器，然后进行部署       
- 系统推荐使用： Ubuntu 18.04
- 初次使用 `./tg-keyword-reply tg-bot-token` , 会将token存到数据库中
- 后面使用 `./tg-keyword-reply` , 无需输入token

后续未开源版本增加了更多群管功能，目前在线机器人 t.me/keyword_reply_bot 和 t.me/keywordreplybot