;-----------------------------------------------------------
　eraTW4.764用潜伏モード追加パッチ1.0readme
;-----------------------------------------------------------
Q,なにこれ
A,eraTW4.764に潜伏モードを追加するパッチです

;-----------------------------------------------------------
Q,潜伏モードって何？
A,外出先の物陰で出来るこっそりうふふです

;-----------------------------------------------------------
Q,なんでこんなものを
A,私室や拠点だけではなく外出先の物陰でこっそりうふふしたいよね。したかった。出来るようにした

;-----------------------------------------------------------
Q,前提となるパッチは？
A,eraTW4.764用画像表示修正パッチv2.1+MYパッチ詰め合わせ
　eraTW関係把握修正パッチ
;-----------------------------------------------------------
Q,詳しい仕様を教えて
A,まとめて書くよ

;-----------------------------------------------------------
・実行方法
「物陰に誘う」コマンド。これで女の子を物陰に誘おう
　ただし通常のうふふ条件に加えて無知か露出癖LV2以上が必要

・潜伏モードの簡単な説明
　普通のうふふだけどその場に他人がいてもばれない
　コマンドを実行する度に上下する潜伏率が0%になると発見される（通常の情事発覚と同じ）
　周りに誰もいないと決してばれることは無い

・潜伏率
　潜伏モード中の体力のようなもの。INFO欄に表示される
　基本的にコマンド実行で低下していく。絶頂時には低下量が3倍になるからイかせすぎに注意。
　潜伏率はキス、継続キス、何もしないのいずれかを実行した際に上昇する
　また継続キス中は絶頂時の低下量すら超える上昇補正が入る。唇を塞いでいれば絶頂させまくっても0にならない優しい仕様
　また現状適切なバランスを模索している段階なので潜伏率の上下量自体抑え目にしてある

・探索モード
　潜伏率が40％を下回った時、その場にいる一番好感度が高いキャラが相手でなくかつその好感度が1500を超えている場合、あなたの気配に気が付いたキャラがあなたを探し始める
　これが探索モード
　探索モードに入ると潜伏率の低下量が大きくなり、キス、継続キス、何もしない実行時の上昇量が小さくなる
　継続キス中の上昇補正は変わらないが絶頂時の低下量をカバーすることは出来ない
　探索モード中は毎ターン探索判定が入り1/5の確率で発見され下記の会話モードへ移行する。6回判定するまでに発見され無かった場合は探索モードは終了し潜伏モードになる

・会話モード
　探索していたキャラにあなたは見つかったがうふふ相手は見つかっていないという極めて危険な状態
　それが会話モード
　低下量は更に大きくなり、キス、継続キス、何もしない実行時の上昇量はすずめの涙に
　更に継続キスの上昇補正まで失われる。それまでの回復行動はもはや意味をなさない
　代わりにこのモード限定で会話コマンド実行時に潜伏率が回復するようになる
　会話キャラが満足して会話を切り上げると会話モードは終了する。ただし相手も好感度が高いのでそう簡単には満足しない
　基本的にターンが経過する度に満足する確率が上昇するので会話しつつ相手が満足するのを祈ろう。運が悪くても20ターンで帰ってくれる

;-----------------------------------------------------------
Q,なんか色々と未完成っぽいけど
A,全ては私の技術不足知識不足によるものです…

;-----------------------------------------------------------
・潜伏モード
　最終的には拠点でも実行可能にしたいと思っている
　さとりなど特定なキャラには容易に発見される、見たいな感じで一部キャラ用の判定も組み込んでみたい
　物陰に誘う判定でも素質による判定を追加したいがやり方がまだ分かっていない
　発情した相手に物陰に連れ込まれる押し倒され潜伏モードもあったらいいな

・潜伏描写
　現状は潜伏場所/モード/潜伏率が表示されているだけ
　二行目にANOTHER_TALKの対話みたいにあなたとターゲット以外の周囲の様子を描写できるようにしたいけど周囲のキャラを参照したりする関数を組めない

・潜伏場所
　数が数だけにノリと勢いで追加したものが多数ある
　基本的にはそのMAPにありそうな場所を追加して目に見える幻想郷をより広くより深くするのが目的のフレーバー

・探索モード・会話モード
　好感度が一番高いキャラが対象だからうふふ中に好感度TOPが入れ替わると強制終了する。本来ならば好感度1500以上なら誰でも良い仕様だったが仕様を実現する関数を組めなかった
　場合によってはあなたではなくうふふ相手が対象になるようにしたい。こいしちゃんと会話してるさとりを机の下で性的に苛めたり出来ると更に幅が広がりそう。ただ別モードにする必要がありそう

・恥情の珠
　本来なら見つかりかねない物陰でのこっそりうふふ。当然恥情の珠の入手が増える処理を入れるべきだけど、やり方が分からない

・うふふ相手以外との交流
　現状は自由自在。本来なら制限を加えるべきなんだけどどこまで加えるかが問題。とりあえず移動を伴うコマンドは縛っている

・潜伏モードという名前
　良い案ください

;-----------------------------------------------------------
Q,バグがあるんだけど？
A,スレで報告してください

;-----------------------------------------------------------
Q,改良とか修正とか追加とか勝手にしていい？
A,どうぞどうぞ

;-----------------------------------------------------------




;-----------------------------------------------------------
Q,これって…作り始めたの2018年だよね？
A,当時は今以上に知識不足だった上私生活が忙しくなって潜伏場所決めた辺りで製作から離れてました
　暇が出来てリハビリで作った月の都MAPがすぐに改良された嬉しさがモチベに繋がってここまで形にすることができました
　eraTW4.764用月拠点追加パッチ【別人改良版】作者様にはこの場を借りて感謝を申し上げます
;-----------------------------------------------------------