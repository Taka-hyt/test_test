# README（共同開発要項）
ver.1.01

## 目的
共同開発での開発フロー、コミュニケーションの取り方、ツールの使い方を体験すること

## 成果物
掲示板アプリ  
サンプル→ [TENKUE HOTEL](https://test.takanori-portfolio.com/)

## 参加要件
- 環境構築が完了し、指定バージョンに揃えられること（詳細は下記）
- ProgateでHTML/CSS、JavaScript、jQuery、Sassを1周していること（もしくはそれと同程度のレベル感）
- GitHubアカウントを持っていること
- お互いを尊重して丁寧なコミュニケーションを取れること
- SlackやGitHubでのレスポンスをできる限り早く行えること（どんなに遅くても24時間以内）

### あると望ましい経験
- GitHubを使用した経験
- 個人で模写をした経験

## 人数とレビュー期間
- 1チーム3名
- メンターのレビュー期間は2週間

## 環境/技術
- EJS
- Sass
- JavaScript または jQuery
- Node.js 12.14.1
- 記法：Scss
- CSS設計：FLOCSSを採用→FLOCSS（https://github.com/hiloki/flocss）
- ソースコード管理：GitHub

## 実装ページ
### [必須要件]
- TOPページ
- ROOMページ
- AREA GUIDEページ
- ACCESSページ
- CONTACT（フォームの送信機能は実装しない）
- Header（ハンバーガーメニュー）
- Footer

### [追加要件]
- 本番環境へのデプロイ

# 共同開発を進める手順
## チーム運営
1. メンターがチームチャンネルを作成して通知します（# 7_2_共同開発_r001。末尾4桁がチーム名です）
1. メンターがキックオフMTGの日程調整を行います。その後はファシリテーターを決めていただいてチームの皆様主導で進めてください。
1. チーム内でまず下記を決めてください
    - ファシリテーター役
    - いつまでに必須要件を終わらせるか（推奨は2週間以内）
    - チーム内ルール3つ（作業時間を週◯時間確保する、毎日進捗報告をする、定期ミーティングをする、など）
1. 上記を決めたらチームチャンネル内で宣言してください

## 開発の流れ
1. 環境構築を完了していることを各自確認
1. 指定バージョンに揃える
1. このリポジトリを下記手順にてクローン
    1. ファシリテーターのGitHubでリポジトリ(A)を作成（リポジトリ名は任意。tenkue-app-r001など）
    1. チームメンバーにリポジトリへのアクセス権限を付与する
    1. $ git clone https://github.com/Tenkue/tenkue_hotel_lp.git
    1. $ cd tenkue_hotel_lp
    1. $ git remote set-url origin リポジトリ(A)のURL
    1. $ git push origin master
1. npmパッケージをインストール
    1. $ npm install
    1. $ npm run start(開発用コマンド)
    1. $ npm run build(本番用コマンド)
1. [Trello](https://trello.com/b/Ov92RvVD)のテンプレートからボードを作成（テンプレートの変更を加えないこと！）してチームメンバー間で共有し、URLをチームチャンネルのトピックに設定
1. 載っている実装ページをそれぞれ実装開始
1. 1ブランチの実装が完了したらチーム内でコードレビューを行ってメンバーからLGTMをもらう（コードレビューは`npm run start`コマンドを叩いてブラウザが立ちがった状態で表示などの確認を行う）
1. チームチャンネル内で、メンターにコードレビューを依頼
1. メンターのLGTM出たらmasterブランチにマージ
1. 次の機能を実装する
1. 5〜9を繰り返す
1. 必須要件の実装が終われば共同開発完了！

## 注意点・特記事項
- クローンしたリポジトリは、チームメンバーいずれかのGitHubにプッシュすること（雛形のリポジトリに変更を加えないこと）
- GitHubとSlackを連携をお願いします
- 雛形のリポジトリには、FLOCSSに沿ったファイル、ディレクトリ構成の実装は完了しています
- クラス名などは自由に付けてもらってもOKです（ただしFLOCSS記法は守ること）
- 技術的な質問はチーム内で共有し調査・解決を図り、解決ができない場合はメンターに質問してください。
- メンターのレビュー対応期間は開発開始から2週間以内です。それを超えたらレビューは行いません（開発自体は継続していただいて問題ありません）
- この共同開発の目的は、技術的なキャッチアップではなく「共同開発での開発フロー、コミュニケーションの取り方、ツールの使い方を体験すること」です
- 開発中は至る所で「ここってどうやるの？」ということが出てくるかと思いますが、①まず自分で調べる②チーム内で相談する、ということを徹底してください
- 開発中のやり取りは共同開発チャンネルにて行なってください。DMなどでやり取りをすると進捗や課題が見えないためフォローができません。

## 作成者
転クエ公式メンター [Taka](https://twitter.com/takaIT3)

## 変更履歴
| ver | date | summary |
----|----|---- 
| 1.0 | 2020/09/06 | 初版作成 |
