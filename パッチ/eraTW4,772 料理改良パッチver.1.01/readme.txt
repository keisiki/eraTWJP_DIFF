eraTW4,772 料理改良パッチver.1.01

バニラ用ですが、以下のパッチも内包しています。
・eraTW4.772用料理アイテム追加パッチ
・eraTW4.772用 はたて口上

※※※導入の際は必ずアップデートしてください。※※※

その際、一部のアイテムが消滅したり別のアイテムに変化します。
▼消滅するアイテム
白米
雑穀
古米
スイカ（の苗） ※以下省略
ナス
サツマイモ
ブドウ
ユリネ
ニンジン
ネギ
こやし
苗は植えているものも消滅します。

▼1.01
抜けている関数の補完（満腹度上昇）と[診察を受ける]際の買い物を改良
一部口上の関数を再設定

▼1.00
●アイテム関連
アイテムの値段を変更しました。
全体的に上方修正してます。

一部アイテムをアイテム番号ごと変更しました。
雑穀→安物食材
古米→上質食材
白米→高級食材
スイカ（の苗）→タマネギ（の苗） ※以下省略
サツマイモ→イモ
ブドウ→カボチャ
ユリネ→ハクサイ
鶏肉→鳥肉

アイテムを追加しました。
獣肉
栄養強化剤

アイテムの所持数制限を一律99個に定めました。

他、使われていないアイテムをコメントアウトしました。

○栄養強化剤
eraTW4.772用料理アイテム追加パッチで足されたものです。
調合で作成できます。
料理を作る際に添加物として混ぜると回復量が上がります。
媚薬等の薬物と分けたので二人で作るときにも使えますし、薬物と併用することもできます。
薬物同様に料理の質が落ちます。

●料理関連
[料理を作る][食事を取る]を中心に料理関連の仕様を一新しました。
料理の品目を増やしました。新たに増やすのも簡単になりました。

料理オプションとイタズラ調味料は廃止しています。
[料理を作る]画面ではメニューや材料、仕込みをまとめて設定します。
面倒な人は「おまかせ」を選択すると作れる料理の中から適当に選んで作ってくれます。

食材は指定されているものの中からどれか一つを使えば作れます。
例えば【肉じゃが】は「獣肉」か「イモ」があればどちらかを使って作れます。

料理作成時に出来栄え（料理の質）が決まります。
料理技能＋食材の品質＋道具の性能（イチョウのまな板）＋ボーナス点＋減点で決定します。
１人のときはあなたの料理技能×２、２人のときはあなたの料理技能＋助手の料理技能になります。
ボーナス点は助手の効果や旬の料理で加点されます。
減点は薬物を混ぜると減点されます。

キャラが食事を取った際は料理の質と味の好みによって採点されます。
高いほど獲得ソースが増えます。低すぎると怒られます。
この際、TARGETか一緒に料理を作ったキャラは獲得ソースにボーナスが付きます。
高得点を出すとかなりのソースを稼げるようになってるので頑張りましょう。

また、一部の料理パラメータによって回復量が変化したり、TSPが回復したり、バフが付いたりします（バフは未実装）
例えば[精力]が付いてるものはあなたが食べると濃厚精液になります。

○固有料理（練習）
現在未実装です。
キャラごとに固有料理を設定してレシピを教えてもらえるようになる予定。

以下はローカル変数または指定変数に移行しました
TCVAR:料理総評価値,料理好評価値,料理悪評価値,料理の時刻,料理の鮮度,料理の味

異物混入.ERBはCOMF413 料理を作る.ERBに統合しました。

キャラデータの味の好き嫌い,助手効果を再設定しました。

落とし物関係の依頼のヒントを再設定しました。
その他料理関連・アイテム関連のイベントも新しい規格を合わせました。
各口上の規格を修正しました。

食事の際の自動集合 @AssembleForMealにバグがあったので修正しました。
（自由行動が持続するバグと同室フラグが立たないバグ）
また、事前にTARGETがいた場合は勝手に切り替わらないようにもしました。

●ショップ関連
通販を始め各ショップの関数を全体的に一新してスッキリさせました。
新たに各アイテムの情報をまとめたITEMDATAを設定しました。
分類や商品としての扱われ方、買ったとき・購入条件等を設定します。
通販と各店舗の在庫の設定にズレが発生するので共有するようにしました。

食料品店で甘味材・獣肉・鳥肉が、酒屋で甘酒が買えるようになりました。


