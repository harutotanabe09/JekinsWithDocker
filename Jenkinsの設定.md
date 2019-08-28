### Jenkinsの設定

・Dockerからイメージをプルするときは、lstイメージを使用する。latestだと落ちる。

### タスクの設定

・古いビルドの破棄は設定しておくこと。データが保持され、重くなる

・ビルドの保存日数:30日、ビルドの保存最大数100日に設定

・Gradleでビルドする設定は、【Invoke Gradle Script】からUse Gradle Wrapperを選択。

　Tasksに【clean build -x test】をセットする。

・Springでビルドしたファイルは、【workspace/＜ワークスペース名＞/build/libs/】にできる
