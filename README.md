# Ascii2dViewer
画像詳細検索サイトのWin用クライアントビューア

/ author: @akatubame
/ date: 2015/02/05
/ version: 0.0.1
/ 使用言語: [AutoHotkey](http://ahkwiki.net/Top)

##■本ソフトの説明

画像の詳細情報データベースを登録している検索サイト「[二次元画像詳細検索](http://www.ascii2d.net/imagesearch/)」の補助クライアントアプリ。  
使用言語は「AutoHotKey」、ソフト名は「Ascii2dViewer」。以下「A2」と略称。

複数画像を一斉検索する場合の効率化目的で作成しました。主な機能は以下のとおり。

- Web上、ローカルの画像ファイルの検索
- 階層構造を持つ詳細情報を自動的に追跡
- 検索した画像、指定画像の詳細情報のそれぞれの一覧表示
- ダウンロードした画像ファイルのリネーム、管理
- 外部からA2を呼び出すホットキー

搭載機能はすべてコンテキストメニューとホットキーの双方から呼び出せる仕様です。  
効率化のためホットキー推奨。特にマウスボタンをホットキーに用いると素早く検索できます。


##■使い方

###検索について

「Ascii2dViewer」を起動すると、メインウィンドウが表示されます。  
まずは検索から始めます。標準では以下の3つの方法で検索の対象となる画像を登録できます。

- [Web上の画像を検索]  
    - 画像ファイルのURLを入力する
        - メニューから「実行」→「URLを指定して詳細検索」と進んで表示されたダイアログにURLを入力

- [ローカルドライブの画像を検索]  
    - 画像ファイル(jpg,gifなど)をメインウィンドウへDrag&Dropする  
    - 画像ファイルのパスをエクスプローラから選択する
        - メニューから「実行」→「ファイルを選択して詳細検索」
	
画像を登録すると自動で詳細検索が始まります。いずれの場合も検索は7秒程度で終了します。  
終了すると、検索した画像一覧がウィンドウの左部に表示されます。

###検索画像一覧

表示された一覧のアイテムを選択すると、選択画像の詳細一覧がウィンドウ中央上部に表示されます。  
この時、検索した元画像のビューアがウィンドウ右下部に表示されるので確認しましょう。  

また、この一覧では、右クリックメニューを呼び出すと指定画像のリネーム、削除などが行えます。

###詳細情報一覧

ウィンドウ中央上部に表示される一覧が詳細情報リストです。  
アイテムを選択すると詳細情報がウィンドウ中央下部に現れます。これがアプリの探すメインの情報となります。  

この時、同時に詳細情報に一致する画像がウィンドウ右上部に表示されます。  
詳細情報の画像はデータベースに登録された類似画像のピックアップであるため、元画像と同じ画像とは限りません。  
(概ね10個程度の類似判定とされた画像が表示されるはずです)  

ウィンドウ右部に2枚の画像が表示されているはずなので、目視で同じ画像かを判断することになります。  
どちらも同じ画像が表示されていれば、中央下部に表示されたテキストが正しい詳細情報となります。

簡単な使い方は以上です。


##■その他の機能

上記の機能の他、任意のウィンドウから「クリップボードURLの検索」などの各種機能を呼び出すことができます。  
以下は標準のホットキーの場合。

- 「Ctrl + Win + F12」でA2メインウィンドウの呼び出し
- 「Ctrl + Win + F11」でクリップボードURLを詳細検索

また、ホットキーには任意のキーを割り当てることができます。以下参照。

	各機能を呼び出すホットキーを自分仕様にカスタマイズすることができる。
	右クリック → 「ホットキーの設定」 から編集GUIを呼び出し、直接文字列を編集する。
	編集後、「変更を保存」をクリックしAEを再起動すると新しいホットキーが有効になる。
	（※この時、重複や存在しないキーなどを指定していると起動失敗するため注意）


##■終わりに  

他にも細かい機能等ありますが、すべて右クリックメニューから呼び出せるので適当に覚えて下さいませ。  
質問や機能の追加要望、バグ報告等は以下へどうぞ。

	Author: akatubame  
	Email: kurotubame5@gmail.com
