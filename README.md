# webptester
The tool can test compatibility user‘s browser display webp image.

WebP是提供无损和有损压缩在网络上图像的新图像格式,WebP无损影像尺寸较PNG格式小26％,有损影像尺寸较JPEG图像相比小25-34％。

##使用方式：

	引入webptester.js，根据特性参数，判断相关特性，其中feature传入'lossy', 'lossless', 'alpha' or 'animation'中得一个特性。callback表示判断后执行的回调方法。

##例子：	
	check_webp_feature('lossy', callback);
	check_webp_feature('lossless', callback);
	check_webp_feature('alpha', callback);
	check_webp_feature('animation', callback);