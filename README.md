# AnarLQRCodeGenerator

####This is an app to convert text string into QRCode.
===================
##Installation
####1.git clone [https://github.com/Kito0615/AnarLQRCodeGenerator.git](https://github.com/Kito0615/AnarLQRCodeGenerator.git)
cd `AnarLQRCodeGenerator/AnarLQRCodeGenerator`
cp `NSImage+QRCode.h` `NSImage+QRCode.m` `/to/your/project`
Add the two files into your project
`#import NSImage+QRCode.h` Then you can use it to Create your own QRCode.
#### There are some methods to create QRCode image.
1)`+ (NSImage *)QRCodeWithText:(NSString *)text;`

2)`+ (NSImage *)QRCodeWithText:(NSString *)text size:(CGFloat)size;`

3)`+ (NSImage *)QRCodeWithText:(NSString *)text QRCodeSize:(CGFloat)size QRCodeForeColor:(QRCodeForeColor)foreColor QRCodeBackgroundColor:(QRCodeBackgroundColor)backgroundColor;`

4)`+ (NSImage *)QRCodeWithText:(NSString *)text QRCodeSize:(CGFloat)size QRCodeForeColor:(QRCodeForeColor)foreColor QRCodeBackgroundColor:(QRCodeBackgroundColor)backgroundColor userIcon:(NSImage *)icon;`

**23/12/2016 Update**

####This method used to recognise QRCode image content

5)`+ (NSString *)QRCodeContentWithQRCodeImage:(NSImage *)qrCodeImage;`

####2.download [AnarLQRCodeGenerator.dmg](https://github.com/Kito0615/AnarLQRCodeGenerator/blob/master/anarlqrcodegenerator.dmg?raw=true)

####3.Update 23/12/2016

###### Add new method to recognise QRCode image content.

##说明
####1.从git安装：git clone [https://github.com/Kito0615/AnarLQRCodeGenerator.git](https://github.com/Kito0615/AnarLQRCodeGenerator.git)
#####（也可以在当前页面直接下载zip）
cd `AnarLQRCodeGenerator/AnarLQRCodeGenerator`  （打开`AnarLQRCodeGenerator`文件夹）

cp `NSImage+QRCode.h` `NSImage+QRCode.m` `/to/your/project`（将`NSImage+QRCode.h` `NSImage+QRCode.m`两个文件拷贝到你的工程目录下并添加到你的工程中）

#####在需要生成二维码的类中引用`#import "NSImage+QRCode.h`就可以了。里面提供了几个方法：
1).`+ (NSImage *)QRCodeWithText:(NSString *)text;` 直接使用文本生成二维码

2).`+ (NSImage *)QRCodeWithText:(NSString *)text size:(CGFloat)size;` 使用文本生成指定大小的二维码

3).`+ (NSImage *)QRCodeWithText:(NSString *)text QRCodeSize:(CGFloat)size QRCodeForeColor:(QRCodeForeColor)foreColor QRCodeBackgroundColor:(QRCodeBackgroundColor)backgroundColor;` 设置文本生成二维码的前景色和背景色

4).`+ (NSImage *)QRCodeWithText:(NSString *)text QRCodeSize:(CGFloat)size QRCodeForeColor:(QRCodeForeColor)foreColor QRCodeBackgroundColor:(QRCodeBackgroundColor)backgroundColor userIcon:(NSImage *)icon;` 设置文本生成二维码的前景色和背景色，并在中间设置头像

2016-12-23更新

####这个方法用来识别二维码内容

5).`+ (NSString *)QRCodeContentWithQRCodeImage:(NSImage *)qrCodeImage;` 识别给定二维码图片内容

####2.直接下载dmg文件[AnarLQRCodeGenerator.dmg](https://github.com/Kito0615/AnarLQRCodeGenerator/blob/master/anarlqrcodegenerator.dmg?raw=true)

2016年12月23日更新，增加识别给定二维码图片功能。
