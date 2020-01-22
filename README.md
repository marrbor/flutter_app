# flutter_app

A new Flutter application.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.

## Tips

テキスト p21 のコマンド `sdkmanager` は、`~/Library/Android/sdk/tools/bin`にある。これをそのまま動作させると、`Exception in thread "main" java.lang.NoClassDefFoundError: javax/xml/bind/annotation/XmlSchema`といったエラーがでる。(デフォルトで使用される Java のバージョンが 9以上であるとき発生する。)

`Android Stdio`に同梱されている`Java SDK`は JDK8 でありエラーを起さない。よって`Android Stdio`に同梱されている`Java SDK`のディレクトリを環境変数`JAVA_HOME`に設定することで、`sdkmanager`を実行することが可能となる。

1. `JAVA_HOME=/Applications/Android\ Studio.app/Contents/jre/jdk/Contents/Home ~/Library/Android/sdk/tools/bin/sdkmanager "system-images;android-27;google_apis_playstore;x86"`
1. `flutter emulators --create --name DevelopAndroid`

