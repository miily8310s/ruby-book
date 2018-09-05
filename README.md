# ruby-bookリポジトリについて
本リポジトリは書籍「プロを目指す人のためのRuby入門」について備忘録である。  
以下は学習に必要なRuby環境構築手順である。

## 環境設定に関して
今回はMac版「Visual Studio Code」（以下VSCode）を使用した。  
Rubyのバージョンは書籍に倣い、`v2.4.1`（rbenv経由）を使用した。

### Ruby本体のインストール
下記URLに従ってインストール。.bash_profileの編集をしないとrbenvからインストールした  
Ruby本体がMacで使用するRubyバージョンと認識してくれない。   

https://designsupply-web.com/knowledgeside/3152/

### VSCodeでデバッグするための手順
1. Rubyエクステンションをインストール  
2. デバッグしたディレクトリを開き、デバッグ画面に移動し、  
初回は構成の追加が求められるためRuby環境を作成する。
3. launce.jsonで`Debug Local File`と書かれたオブジェクト内のprogramのパスを  
`${workspaceRoot}/デバッグしたいRubyファイル`に変更する
4. このままだとデバッグエラーが出るため追加で以下のgemをインストールする
   - ruby-debug-ide
   - debase

（参考URL）※書籍著者本人による記事  
https://qiita.com/jnchito/items/acc7b4b0a31330982bb0
