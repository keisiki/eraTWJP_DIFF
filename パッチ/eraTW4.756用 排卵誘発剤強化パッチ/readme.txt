2020/08/23
　eraTW4.756用 排卵誘発剤強化パッチ

◆対象環境
　eraTW4.756

◆説明
・排卵誘発剤入りお茶は料理を作れるように
　>>270スレ目>>616からの
・危険日に排卵誘発剤を使うと妊娠確率が下がるのを修正
　>>270スレ目>>703からの

◆導入方法
　展開したフォルダをそのままeraTW4.756に上書きしてください
　必ずバックアップを取るようお願いします

◆雑談
　パッチの修正・利用はご自由にお願いします

◆詳細
ERB/
┗イベント関連
　┗妊娠関連
　　┗CYCLE.ERB ; 危険日に排卵誘発剤を使うと妊娠確率が下がるのを修正
　　　　　　　　; 排卵誘発剤による確率変更前と後のコードを分離
　　　　　　　　　; 安全日の判断をESTRUS_CYCLEに依存してるコードが多かったのでこんな形にした
　　┗PREGNANCY.ERB ; 妊娠確率計算に使う関数を変更（CYCLE.ERB修正関連)
┗コマンド関連
　┗COMF
　　┗日常系
　　　┗COMF331 お茶を淹れる（薬入り）.ERB ; 排卵誘発剤入りお茶を飲むときの処理
　　　┗COMF413 料理を作る.ERB ; 排卵誘発剤入りお料理を作れる
　　　┗COMF425 薬を盛る.ERB ; 排卵誘発剤入りお茶を作れる
　　　┗FOOD.ERH ; DISH_DRAG_排卵誘発剤を追加
　　┗異物混入.ERB ; 排卵誘発剤入りお料理を作れる
┗口上・メッセージ関連
　┗EVENT_MESSAGE_COM500.ERB ; 排卵誘発剤入りお料理を食べるときのメッセージを追加
┗ステータス表示関連
　┗INFO.ERB ; 排卵誘発剤入りお料理を持ってると料理の名前のあとに(排卵誘発剤)が出力