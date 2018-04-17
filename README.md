VSCE - FormatNovel README
=========================

小説のルールに基づき文書を整形する、Visual Studio Codeの機能拡張です。  
マイクロソフトが公開している[サンプル](https://github.com/Microsoft/vscode-extension-samples)を参考にしています。

## Usage

`Format Novel` コマンドを実行すると、下記のルールに基づき文書をフォーマットします。

(1) 行頭に全角スペースを挿入します。ただし、下記と一致する行を除きます。

* 鉤括弧(「、『)で始まる行
* Markdownの見出し記号(#)で始まる行
* 既に全角スペースが挿入されている行
* 空行

(2) 全角の感嘆符(！)、疑問符(？)のあとに全角スペースを挿入します。ただし、下記と一致する場合を除きます。

* 直後が感嘆符(！)、疑問符(？)、鉤括弧(」、』)、半角スペースの場合
* 既に全角スペースが挿入されている場合

## Command

いずれかの方法でコマンドを実行してください。

* コマンドパレットを開いて(<kbd><kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd></kbd>) '`Format Novel`' と入力する
* エディタ内で右クリックし、コンテクストメニューから '`Format Novel`' を選択する
* <kbd><kbd>Shift</kbd>+<kbd>Alt</kbd>+<kbd>/</kbd></kbd>とショートカットを入力する

なお、コマンドが有効になるのは、言語モードがMarkdown形式またはプレーンテキスト形式の場合のみです。
