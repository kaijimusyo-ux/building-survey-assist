建物調査アシスト Ver.0.5 — PWA試作版

【重要】ZIPをiPhoneの「ファイル」アプリで展開しても、PWAとしてインストールできません。
HTTPS対応のWebサーバーにZIP内のファイルをすべて配置し、iPhoneのSafariで index.html を開いてください。

【導入例：GitHub Pages】
1. GitHubでリポジトリを作成（公開リポジトリに実案件データは置かないでください）。
2. このZIP内の index.html / sw.js / manifest.webmanifest / icon-192.png / icon-512.png をリポジトリのルートにアップロード。
3. Settings > Pages > Build and deployment > Deploy from a branch > main / (root) を選択。
4. 発行された https://.../index.html をiPhoneのSafariで開く。
5. Safariの共有から「ホーム画面に追加」。
6. ホーム画面から起動し、サンプル敷地を表示。その後、機内モードにして再起動テスト。
※初回に全ファイルの取得とキャッシュ登録が必要。iOSのストレージ整理でキャッシュや保存データが消えることがあります。
※Github Pages等にアプリ本体を公開しても、作図したデータは端末内に保存されます。アプリ本体に顧客情報や実案件SIMAを同梱しないでください。

【機能】サンプル敷地、SIMA読み込み、建物CAD作図/手書き、辺の寸法メモ、JSONバックアップと復元、DXF出力、SIMA試験出力。
【制限】SIMA形式は実ファイルで追加検証が必要。手書きは概略形状。柱芯オフセットは参考計算のみ。法的求積・閉合差・同期・写真管理は未実装。
【データ保護】端末内保存はブラウザ領域に依存します。現場終了時にJSONバックアップを必ず出力してください。端末間自動同期はありません。
