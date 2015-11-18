# webptester
The tool can test compatibility user‘s browser display webp image.

WebP（发音 weppy），是一种支持有损压缩和无损压缩的图片文件格式，派生自图像编码格式 VP8。根据 Google 的测试，无损压缩后的 WebP 比 PNG 文件少了 45％ 的文件大小，即使这些 PNG 文件经过其他压缩工具压缩之后，WebP 还是可以减少 28％ 的文件大小。

因为webp在一些浏览器上不能使用，所以出现了该工具来判断浏览器支持webp的兼容性，做出正确的动作。

webp官方地址 https://developers.google.com/speed/webp/

##使用方式：

	引入webptester.js，根据特性参数，判断相关特性，
	其中feature传入'lossy', 'lossless', 'alpha' or 'animation'中得一个特性。
	callback表示判断后执行的回调方法。

##例子：	
	// 是否支持有损压缩的webp
	check_webp_feature('lossy', callback);
	// 是否支持无损压缩的webp
	check_webp_feature('lossless', callback);
	// 是否支持有alpha的webp
	check_webp_feature('alpha', callback);
	// 是否支持有animation的webp
	check_webp_feature('animation', callback);