# web版App

创建工程参照官方文档：https://flutter.dev/docs/get-started/web

主要设计命令：

    flutter channel stable  flutter切换到stable版本
        
    flutter create myapp  创建工程：

    cd myapp 打开工程

    flutter run -d chrome 运行到web上

    


## 常见错误

1、部分库不支持null-safety版本，运行后会报错如下：

Flutter--Error: Cannot run with sound null safety, because the following dependencies don't support null safety:

Error: Cannot run with sound null safety, because the following dependencies
don't support null safety:
flutter sdk提示不是支持 null safety模式

解决方法：

    flutter run --no-sound-null-safety -d chrome

    flutter build apk --no-sound-null-safety

