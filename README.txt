Room Display (KY-41C用 WebViewアプリ)

1. app/src/main/java/com/example/roomdisplay/MainActivity.java の
   START_URL を自分のWebアプリのURLに書き換える
2. GitHubにアップロードすると、Actionsが自動でAPKを作る
3. Actions > 最新の実行 > Artifacts の room-display-apk をダウンロード
4. zipを展開して app-debug.apk を取り出し、次を実行
     adb install app-debug.apk
     adb shell am start -n com.example.roomdisplay/.MainActivity
