eraTW4.800用 CHARA_SLEEP改良＆口上拡張+α

●注意事項
・以下のファイルは他のパッチを取り込んだ状態を前提にしてます
移動.erb	映姫様詰め合わせV4
COMMON.erb	eraTW4.800用 虫捕りパッチver.0.70β
KOJO_MESSAGE.ERB.erb	eraTW4.800用 虫捕りパッチver.0.70β
口上テンプレ	eraTW4.800用 虫捕りパッチver.0.70β

その他のパッチ（TWモブ子店員パッチ、別キャラ孕ませ）は競合しているので留意してください。
放尿解放のみ、入れた場合を想定してコメントアウト状態になっています。


●改良箇所
@SLEEP_CHARA
　色々とっちらかってたのを整理
　発生しなくなってた口上や死に分岐を修正
　地の文を少し改良
@起床就寝処理
　デート時帰宅処理をSLEEP_CHARAでまとめて行うように
　うふふ中、デート中に寝る場合の分岐（地の文）を加筆
@寝室から追い出し
　追い出し設定を@寝室許可でひとまとめに
　複数のキャラが寝室を共有している場合の処理を設定
　追い出し関数内で口上を呼び出すように
@EVENTCOMEND
　おやすみ口上改良に伴ってちょっと改良
@部屋に忍び込む
　追い出される処理を修正
@COMMON
　ENDUFUFU_ALLを新設

●口上テンプレ拡張箇所
▽拡張
おやすみ口上
　デート中やうふふ中等の発生タイミングによる分岐をサンプルに追加
帰宅口上
　うふふ中に帰る分岐をサンプルに追加
　部屋に誘われる分岐を追加（4〜6）
　拠点に泊めてもらう分岐を追加（7〜9）
　疲れて帰る時の分岐を追加（10）
陥落素質取得口上
　キス魔、自慰狂い、ポルチオ性感の分岐を追加（6〜8）
　キス魔、自慰狂いは地の文を加筆
　[恋慕]等も表示するタイミングをちょっとずらしました
　おもらし癖(9)は放尿解放パッチを入れたうえで、
　EVENTTURNENDのコメントアウトしている箇所を解くと使えるようになります

▽新設
自由行動に付き合う（日常コマンド）
自由行動中（イベント）
ハッピーニューイヤー
技能レベルアップ（技能素質取得）
共通のデイリーイベントに口上を付けられるように
　現状は→の3つ（02,夢精、04,物思い、12,特訓）
　口上側で地の文も変えられます
　02,夢精は獲得JUELも変えられます

●その他の修正
買い物（自由行動）の発生時間を9時〜19時に限定
演奏（自由行動）が発生しなくなっていたのを修正
