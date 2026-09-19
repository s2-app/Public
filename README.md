# Ss Tools

個人開発した Windows 向けユーティリティ（**Ss シリーズ**）のコンパイル済みアプリを配布しています。

- 対象OS: **Windows 10 / 11 (x64)**
- 形式: **自己完結単体 exe**（.NET ランタイムのインストール不要）
- ソースコードは非公開です。ここでは実行ファイルのみを配布します。

## ダウンロード

最新版は **[Releases](../../releases)** から入手できます。

各アプリの zip をダウンロードして展開し、中の `.exe` を実行してください。

## 収録アプリ（v1.0.0）

| アプリ | 概要 |
|---|---|
| 🗄️ SsDbClient | DB接続・SQL実行・データ集計・DB定義出力 |
| 📄 SsFileList | フォルダ内ファイルの一覧化・出力 |
| 🔊 SsAudioSwitcher | 再生/録音デバイスのワンクリック切替 |
| ✂️ SsFileSplitter | 大容量ファイルの分割・結合 |
| 🏠 SsSwitchBot | SwitchBot デバイス・シーン操作 |
| 💬 SsMsgBoxTest | MessageBox の見た目・戻り値確認 |

各アプリ名をクリックすると詳細（機能一覧）が展開されます。

<details>
<summary><strong>🗄️ SsDbClient — データベースクライアント</strong></summary>

Oracle / SQLite / SQL Server / ODBC / OleDb に対応した汎用DBクライアントです。

- テーブル・ビューなどの一覧表示とデータ閲覧
- SQL エディタでのクエリ実行、SQLフィルタ・SQL解析（Oracle）
- データの集計（グラフ表示付き）
- DB定義の出力、データの出力・取込・作成（旧 SsDbTools の機能を統合）
- 接続情報は DPAPI で暗号化して保存（平文保存なし）

</details>

<details>
<summary><strong>📄 SsFileList — ファイル一覧作成ツール</strong></summary>

指定フォルダ配下のファイル情報を一覧化するツールです。

- フォルダ選択→検索でファイル一覧を収集（サブフォルダ再帰対応）
- ファイル名・サイズ・更新日時などの列をカスタマイズして出力
- 収集結果同士の比較・マージ、既存有無チェックにも対応

</details>

<details>
<summary><strong>🔊 SsAudioSwitcher — オーディオデバイス切替ツール</strong></summary>

タスクトレイに常駐し、再生/録音デバイスを素早く切り替えます。

- トレイアイコンを**左クリックで出力デバイスを順送り切替**、**右クリックでミキサー画面**を表示
- 出力・入力それぞれにホットキーを割り当てて循環切替が可能
- ミキサー画面で音量調整・ミュートも操作可能
- Windows起動時の自動起動に対応

</details>

<details>
<summary><strong>✂️ SsFileSplitter — ファイル分割・結合ツール</strong></summary>

大容量ファイルを指定サイズ／個数で分割します。

- ファイル・フォルダをドラッグ＆ドロップで指定可能
- 分割数 or 分割サイズ（KB/MB/GB単位）を指定
- 分割後の結合用バッチファイルを自動生成
- 分割前にプレビューで結果を確認可能

</details>

<details>
<summary><strong>🏠 SsSwitchBot — SwitchBot コントローラー</strong></summary>

SwitchBot API を使ってデバイス・シーン・グループを操作します。

- デバイス一覧表示、個別デバイスへのコマンド送信（赤外線リモコン／エアコン対応）
- シーンの一覧・実行、グループ編集
- タスクトレイ常駐（`--tray` 起動でスタートアップから自動起動）
- コマンドライン実行にも対応（`SsSwitchBot.exe "シーン名"` や `"デバイス名" "ボタン名"` でショートカットやタスクスケジューラから呼び出し可能）

</details>

<details>
<summary><strong>💬 SsMsgBoxTest — MessageBox 表示テストツール</strong></summary>

`System.Windows.Forms.MessageBox` の見た目と戻り値を確認するための開発支援ツールです。

- アイコン（エラー／警告／インフォメーションなど）・ボタン構成・タイトル・メッセージ文を指定して表示
- よくあるパターン（エラー／警告／インフォメーション）をワンクリックで設定
- 実際に表示した際の戻り値（OK/Cancel等）を確認できる

</details>

## 使い方

1. Releases から対象アプリの `*-win-x64.zip` をダウンロード
2. 任意のフォルダに展開
3. `.exe` をダブルクリックで起動

> ⚠️ 初回起動時に SmartScreen の警告が出る場合があります（署名なしのため）。「詳細情報」→「実行」で起動できます。

## ライセンス / 免責

個人開発・無保証で提供しています。利用は自己責任でお願いします。
