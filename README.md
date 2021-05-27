# めうちきりんのメトロポリス

**「めうちきりんのメトロポリス」** は、文章生成にカットアップと自然言語処理の知見を活用した、ショートショート形式のサウンドノベルゲームです。  

公式サイト: [https://myochikirin.ippee-music.com/](https://myochikirin.ippee-music.com/)  
公式サイトリポジトリ: [https://github.com/ippee/novel_game_hp](https://github.com/ippee/novel_game_hp)  

技術解説記事: [https://ippee-music.com/tech/myochikirin/](https://ippee-music.com/tech/myochikirin/)

![title](./assets/title.jpg)  

## 使用技術
### 概要
- フロントエンド
  - **Vue.js**
    - UI構築
    - スクリプト・エンジン開発
- バックエンド
  - **Rust**
    - **tauri**
      - ウィンドウ表示
      - セーブ＆ロード機能
    - **rodio**
      - オーディオ管理
        - BGM/SEの再生、音量調整
- 文章生成
  - **Python**
    - カットアップ
    - 自然言語処理

### 構成
詳細は各フォルダ内にあるREADMEを参照。

- フロントエンド（./src/）
  - assets/
    - 静的なファイルを保存するフォルダ
  - components/
    - UIをコンポーネント単位で分割したファイル群
  - mixins/
    - 各コンポーネントで再利用する.js形式の機能やデータ
  - router/
    - 各ページのルーティングを管理するフォルダ
  - App.vue
    - vue-routerの描画先となるコンポーネント
  - main.js
    - Vueインスタンスを作成する.jsファイル
- バックエンド（./src-tauri）
  - audio/
    - ゲームで使用する音源を管理するフォルダ
  - icons/
    - ゲームのアイコンを格納するフォルダ
  - savedata/
    - json形式のセーブデータ
  - src/
    - Rustのソースコード

## 文章生成について
文章生成の大きな流れとしては、まず既存の文章を形態素解析によって分割し、それらを一定のルールでバラバラに組み替えたり、N階マルコフ連鎖によって短いセンテンスを生成します。  
そこらか個人的に良いと感じたセンテンスをピックアップし、それらを直感的に組み合わせることによって本文を作成しました。  

詳しい文章生成の仕組みについては、別リポジトリにて解説を行う予定です。  

## 開発環境
### Windows
- OS: Windows 10 Home

### Mac
- OS: Catalina 10.15.7