eraTW4.632用下半身描写修正+αパッチ



スカートめくりの地の文がまだ短くできるかと思い修正しました。UNDER_SKIRT_DESCRIPTIONって便利ですね。
それに伴いUNDER_SKIRT_DESCRIPTION、SLIT、HIPの加筆を行いました。
あと華扇口上の膝枕とスカートめくりも修正しました。ライセンスの記述がないので問題かもしれませんが……

HIPの汗で透けたを個別に判定するために関数オブジェクト内の透けるを透ける(前)と透ける(後)に分離しました。
透ける(前)が今までの透けるで、透ける(後)は尻肉がパンツで透けるかどうかで判定しています。(後)はＧストリング、Ｔバック、前張りなどでは透けないとしています。
