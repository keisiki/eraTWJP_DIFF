eraTW4.756用画像表示修正パッチ V1.05

・概要
TW4.754用画像表示修正パッチの続きです。
就寝後の自慰イベントが、画像表示するとログが長くなる問題を解決するため、
OPTIONで就寝後の自慰画像表示有無を選べるようにしました。デフォルトはONです。
さらに一人ずつじっくり画像を見たい人(というか私)のため、一人ずつ行送りが止まるようにしました。不評なら戻す
他更新点として、能力表示時差し替え画像の変更ができるようになりました。
これで差し替え画像の変更や発見がしやすくなるはずです。うちの環境だと何人か表示されてないけど…

・導入環境
以下の環境でパッチを導入してください
# TW4.756

・導入方法
展開したフォルダをそのままeraTW4.756に上書きしてください。
必ずバックアップを取るようお願いします。

・連絡事項
FLAG:1071を使用しました。個人改造で使用している人はご注意を
このパッチはv1.03、v1.04の更新内容を含んであります。
それ以下のバージョンはTW4.756に同梱済みです。

・詳細
eraTW4.756
v1.05
CSV/
┗FLAG.csv
　　FLAG:1071を自慰画像表示判別用に使用
ERB/
┣SHOP関連/
┃┗OPTION.ERB
┃　　改行を削除
┃　　自慰画像表示の選択を追加
┣イベント関連/
┃┗AFTERTRA.ERB
┃　　自慰画像の表示をフラグ制御するように変更
┃　　自慰イベント後行送りを停止するよう変更
┗ステータス表示関連/
　┗能力表示.ERB
　　　差し替え画像がある場合、選べるよう選択肢を増設
　　　画像表示後の改行をIMEGE.ERBで行うように修正

v1.04
ERB/
┗ステータス表示関連/
　┗IMAGE.ERB
　　　画像表示OFFの場合自慰画像を表示しないように変更

v1.03
ERB/
┗ステータス表示関連/
　┗IMAGE.ERB
　　　自慰画像が正しく表示されない問題を修正

eraTW4.754
v1.02
ERB/
┗ステータス表示関連/
　┗IMAGE.ERB
　　　別画像のエフェクトが正しく表示されない問題を修正
　　　別画像を選択していた場合、能力表示画面も別画像が表示されるよう変更

v1.01
ERB/
┗ステータス表示関連/
　┗IMAGE.ERB
　　　テキストタグボタンの間隔が負の値にならないよう修正

v1.0
CSV/
┗_fixed.config
　　TW4.753以前のものに修正
ERB/
┣グラフィック表示ライブラリ/
┃┗グラフィック表示.ERB
┃　　画像サイズを元画像の高さを参照せず、デフォルトキャラ画像横幅を参照するように
┃　　画像反転時、縦幅は反転しないように
┃　　縦位置の計算を変更、"一行の高さ"を参照するように
┃　　ピクセル自動改行の計算を変更
┗ステータス表示関連/
　┣IMAGE.ERB
　┃　画像サイズ比の計算を変更、よりウィンドウ幅に合うように
　┃　テキストタグボタンの間隔計算を変更
　┃　時間停止、フレームの描画の一部を省略
　┃　ステータス画面の画像表示でフレームが表示されるように
　┃　他細々とした表記やインデントを修正
　┗キャラ描画共通.ERH
　　　使用しない変数を削除
emuera.config
　TW4.753以前のものに修正