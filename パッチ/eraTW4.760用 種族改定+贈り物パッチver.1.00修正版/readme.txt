eraTW4.760用 種族改定+贈り物パッチver.1.00

※※※※※※※※※※※※※※※※※※※※※※
※適用する際は必ずアップデートしてください※
※※※※※※※※※※※※※※※※※※※※※※

※修正版
妊娠関連フォルダが抜けてたので修正しました。

■種族改定
・種族素質の設定を整理しました。
［妖怪］［幽霊］［人形］［追加種族］を新設
［鬼］［天狗］は［妖怪］に移動
［巫女］［魔法使い］［蓬莱人］は［追加種族］に移動
［非生物］は［幽霊］［人形］に分割して移動
［追加種族］として［メイド］を新設
他、［人間］［妖怪］［神霊］［幽霊］［人形］［追加種族］を細分化

・最も影響のある妊娠関連については以下の通り。
［妖怪孕ませ］をちゃんと［妖怪］に効果があるように
［鬼］［天狗］を孕ませても［妖怪孕ませ］は取得できないが、［妖怪孕ませ］があると［鬼］［天狗］の妊娠率に少し効果があるように
［幽霊］［人形］に対しては［幽霊孕ませ］［人形孕ませ］を新設
［巫女］［魔法使い］に次ぐ形でメイド孕ませボーナスも設定（素質ではなく料理経験）
ちなみに5種族に届きやすくなったが［幽霊］［人形］は元々確率が低いので狙って取るものではない
［仙人］［天人］［月人］［魔界人］を［人間］と分けて妊娠率を若干下降修正
ハーフの妊娠確率は人間の妊娠確率との平均値に

・その他の影響は以下の通り。
桃色の風や調合アイテムの効果が無かった［非生物］を［人形］のみにしたので［幽霊］には効果があるように
依頼『懲らしめて！』の討伐対象を改良
スカウターの倍率を改良
能力表示の種族欄の表示方法を改良
モブ子の種族に対応

それ以外は一部の種族が変わったキャラへの影響になります。
とは言ってもそこまで大きく変わったキャラは少ないです。魔理沙が［人間］、アリス等が［妖怪］に分けられたくらい。

■贈り物
ひとまず設定したいところは完成しました。
やれそうなことは気が向いたときに作るかも。
贈り物データや追加要素作りたい人はご自由に。

▼更新履歴
・ver1.00
　旧作キャラを含め全員分の感性を設定
　形容詞データを更新
　魔法の森の土産屋を香霖堂表記に

・ver0.53
　旧作キャラ以外の感性を設定
　これによって採点機能が機能します
　採点時の共通設定を修正
　贈り物形容詞データ更新
　贈り物本体データを修正
　@AREA_SETBITを改良

・ver0.12
　とりあえず全地域に土産屋を設定
　贈り物本体データを一通り設定
　採点時の共通設定を設定
　※キャラデータを設定してないのでまだ採点機能は実質機能してません

●やれそうなこと
一人でも土産屋を利用できる
　CFLAG:贈り物ストックに一つだけストックしておき、デート中任意のタイミングでプレゼントできる。

拠点でも土産屋を利用できる
　同行人数が1人ならプレゼントできる。住民にはプレゼントできない。
　問題は場所が決まらない。（人里とか）

プレゼントしてもらえる
　なんらかのタイミング（デート帰りイベント？）でデート相手から贈り物を貰える。キャラごとにパターンが変わる。
　CFLAG:渡した贈り物を参照して誰から何を貰ったか（各1つずつまで）確認できる。
　1つ選んでお気に入りにできる。
　ITEMフラグに設定すれば周回で消えない（銀の手は消えない！）

半額セール
　デイリーイベントで特定地域の土産屋で半額セールが発生する。

霖之助や地域ごとの台詞
　店によって地の文に台詞が入る。

香霖堂裏メニュー
　なんらかの条件等で裏メニューが見れる。
　裏メニューは地域制限がなく全てのパターンで商品が生成される。（オールブルー）

品揃えが増える
　なんらかの条件で土産屋に並ぶ商品の数が増える。

値下げ・値切り
　なんらかの条件で土産屋の値段が割引される。

口上テンプレの実装
　大変……。

能力表示に表示
　衣装の欄？

