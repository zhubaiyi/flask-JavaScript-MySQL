使用flask作为后台逻辑的Paddle OCR号牌检测系统，web前端使用模板引擎jinja2，移动端使用微信小程序js作为前端页面；

web部分使用的是本地inference模型（pychar可以自行下载部署），移动部分则调用百度paddleocr接口进行调用，需要自行注册以及调用

这是一个通过flask后台使用百度云识别api进行图片号码牌识别的一个项目，flask为后台程序，另一个是前端程序
其中使用的技术是flask的技术，以及微信小程序的JS技术
目前实现了上传、上传的同时识别的功能，以及根据识别的内容进行搜索，可以对识别的结果进行复制，对图片进行下载的功能。
但是目前没有实现分发功能（即无法对同一个号牌但是不同赛事以及用户进行分类的输出数据），目前这个功能已经有相应的研究生开发出来了，使用的是Django
