;--------------------------------------------------
;●パチュリー・ノーレッジ口上＠erablue_resort用
;　――れあどめ
;--------------------------------------------------
;初期作者：NEOの人/鵺野アラタカ
;作成日：下記更新履歴を参照
;--------------------------------------------------
;当口上の概要、コンセプト、メモ、使用フラグに関しては、更新履歴下の「メモ」を参照
;--------------------------------------------------

;--------------------------------------------------
;●ライセンスについて
;--------------------------------------------------
;	+----+----+-------------------------------------------+
;	|番号|許可|ライセンス内容                             |
;	+----+----+-------------------------------------------+
;	|   1| ○ | 処理上のバグ修正                          |
;	+----+----+-------------------------------------------+
;	|   2| ○ | 新規機能追加による内容改変                |
;	+----+----+-------------------------------------------+
;	|   3| ○ | バランス調整による内容改変                |
;	+----+----+-------------------------------------------+
;	|   4| ○ | 口上の誤字・脱字の修正                    |
;	+----+----+-------------------------------------------+
;	|   5| ○ | 口上の新規追加・加筆                      |
;	+----+----+-------------------------------------------+
;	|   6| ○ | 既存口上の改変                            |
;	+----+----+-------------------------------------------+
;	|   7| ○ | 改変した口上の自由な再配布                |
;	+----+----+-------------------------------------------+
;	|   8| ○ | 口上内容の転載（erablue_resort内部に限る）|
;	+----+----+-------------------------------------------+
;	|   9| ○ | erablue_resort本体への収録                |
;	+----+----+-------------------------------------------+
;
;--------------------------------------------------

;--------------------------------------------------
;●更新履歴
;--------------------------------------------------
;	ﾊﾞｰｼﾞｮﾝ	ｺｳｼﾝﾋﾂﾞｹ		ｶｲﾀﾋﾄ					ﾅｶﾐ
;	Edit	Date			Author					Reason
;	001		2024/10/16		NEO/鵺野アラタカ		0.00。作成開始。
;													　楽しませていただいてるので、ぐらぶる知らないなりになんかしたくなった。
;													　目標は「現在のテンプレファイルを全部使う」。
;	002		2024/10/23		NEO/鵺野アラタカ		0.01。公開。
;													　バトル関連：
;													　　戦闘ステータス設定関連
;													　　固有アビリティ関連
;													　　固有奥技関連
;													　　→仮設定。技の概要はともかく、威力や消費を調整する可能性大。
;													　設定：
;													　　ステータス設定
;													　　パラメータ設定
;													　　商業区_固有店舗処理（※名称を設定しただけだよ）
;													　イベント：
;													　　イベント発生時
;													　コマンド：
;													　　オートコマンド発動時
;	003		2025/06/17		NEO/鵺野アラタカ		0.02。なんも終わらん……
;													加筆箇所はメモってたけど「いっぱい」で終わりにしておきます
;													色々未完成の部分が極めて多いのですが、「いったん出す！」という決意のもと、コメントアウトなどで対応しています
;													川上稔『終わりのクロニクル』がなんかあるってマジ！？
;
;--------------------------------------------------

;--------------------------------------------------
;●概要/コンセプト（ver20241015）
;--------------------------------------------------.
;〇はじめに
;　以下はNEOの人のメモ、覚え書きであり、加筆者さんは無視してもいい。
;
;〇性格/陥落前/前提
;　本があれば幸せ。本の虫。理屈っぽい。
;　冷静沈着……というよりは、外界に基本的に興味がない、と言ったほうが正しいだろうか。
;　雰囲気は暗くてじめじめしているが、別に当人は暗くない。
;　（あまり積極的にはやりたがらないだろうが）フィールドワークなんかもこなす。
;　知識はほぼ書物から得ており、なんなら「目の前の事実よりも本に書いてあったことを優先」したりするかも。
;
;〇性格/陥落後
;　あんまり、「好き好き大好き～❤」となるタイプではない。
;　「パチェ、と呼んでもいいわ」って言われたり……したいわね！
;　無論のこと、これらは「陥落しても変わらない」事項もある。
;
;〇身体について
;　病弱、喘息持ち。
;　それはそれとして、身体はムッチムチ。
;　全然動いてないので筋肉量がなく、やわらか。おにくぷにぷに。
;　陥没乳首。
;　/
;　eratohoから伝統的に「全身敏感で体力が低い上に回復遅い」設定。
;　古くは貧乳派と巨乳派が分かれていたが、近年はムチムチボディが多いか（貧乳ぱっちぇさん、あまり見なくなったねえ）。
;　CSV側で小柄爆乳肉感的安産型なので、それに従う。
;　/
;　陥没乳首にできるのは趣味だよ。
;
;〇その他
;　CSV設定だと調合Lv1を持っているが、彼女は調合が苦手らしい。
;　解釈すると、「苦手だが知識はある」という感じだろうか？
;
;〇文章規範
;・前提
;　　オーナーは[オトコ]あなたで、パチュリーは女（非[オトコ]）とする。
;・地の文/マスターの言動
;　視点をオーナーに固定した三人称の文体を基本とする。
;　『オーナーはプレイヤーの分身である』ことを意識し、可能な限り心情描写は省くものとする。
;　オーナーの命令/お願いは、ダブルクォーテーション（“”）でくくるか、『そういうお願いをした』という文章とする。
;　まあこのあたりはアバウトというかそこまで統一してないのだけど、
;　『プレイヤーはちっとも惜しいと思っていないのに、オーナーが“惜しい”と考える』……このような事態を避ける。
;・喘ぎ
;　オホ声とか……いいよね！！！
;・ハートマーク
;　いっぱいあるほうが……えっちだよね！！！
;
;・コンパチ
;　出ない“書く予定”よりは、出るコンパチ。
;　ただし、同じ『初回口上』が二度も三度も出ないように気を使うこと。
;・コメントアウト
;　多めの予定です。
;
;--------------------------------------------------

;--------------------------------------------------
;●キャラデータ（ver20241015）
;--------------------------------------------------
;〇基礎情報
;　番号：1147
;　名称：[動かない大図書館]パチュリー
;　名前：パチュリー・ノーレッジ
;　種族：その他（魔法使い）
;　原作：東方project
;
;〇BASE/体格関連
;　　体力　：1600
;　　性欲　：1600
;　　身長　：1490（149センチ）
;　　体格　：小柄
;　　バスト：爆乳（G～I)
;　　体型　：肉感的
;　　下半身：安産型
;　　Ｂ　　：92.4（Ｈカップ）　※ＢＷＨは「このくらいになる」なのかな？
;　　Ｗ　　：60.8
;　　Ｈ　　：94.9
;
;〇身体的特徴（フレーバー）
;　　CSV設定なし
;　　下記の如き思想で口上独自設定を行う
;　　　陰毛：濃い。くさそう（確信）
;　　　乳首：大きめ。土台となる乳房が爆乳にしてもデカい。
;　　　乳輪：大きめ。同上。
;　　　膣内：締まりはやや緩そう……あえて分類するなら巾着系かもだが、名器レベルかは微妙かしら。設定しない。
;　　　クリ：平均的
;　　　ほくろ：乳首横。乳押し。
;
;〇服装
;　　パチュリーのパジャマワンピース
;　　　上半身服
;　　　下半身服（めくり可）（下着抜き取り可）
;　　　ブラ着用　下着着用
;
;〇同行者
;　　[華人小娘]紅美鈴_10%
;　　[名もなき小さな悪魔]小悪魔_30%
;　　[完全で瀟洒な従者]十六夜咲夜_10%
;　　[永遠に紅い幼き月]レミリア_20%
;　　[悪魔の妹]フランドール_10%
;
;〇知識
;　　性知識　：Lv2
;　　調合知識：Lv1
;　　魔法知識：Lv3
;　　運動クソザコナメクジなので水泳レベルを-1とかにしてもいい気はするが……まあ案外動けるんだよね、本のカドで殴ったり。
;
;〇TALENT/素質
;　　[オンナ][処女][Ａ処女]
;　　[大人しい][夜更かし癖][寝ぼすけ][無関心][習得早い][舌使い]
;　　[Ｃ敏感][Ｖ敏感][Ａ敏感][Ｂ敏感][Ｓ敏感]
;　　[濡れやすい][回復遅い][禁断の知識][サウナに弱い][冷静][早イキ]
;　　[魔法を使う程度の能力]
;　　+[陥没乳首]
;　　+年齢系素質[]（彼女は100歳をこえている）
;
;〇ABL/能力
;　　初期能力なし
;
;〇EXP/経験
;　　初期経験なし
;
;〇弱点コマンド
;　　CSV設定なし
;　（以下、口上独自設定）（全身弱点早イキの性的クソザコナメクジなので、色々設定してもいい気はするが……）
;　　乳首当てゲーム
;　　知識を教える
;　　以下、ランダム設定
;
;〇その他
;　　プレゼント好み：本
;　　属性：水
;　　得意武器：杖
;　　初期ステタイプ：バランス
;
;
;====================================
;

;--------------------------------------------------
;●使用フラグ
;--------------------------------------------------
;〇特定状況口上用フラグ
;　0-99までのはず
;　  0：（この辺は重要フラグに使いたいな～）
;　  1：
;　  2：
;　  3：
;　  4：
;　  5：
;　  6：
;　  7：
;　  8：
;　  9：
;　 10：オーナーによる初絶頂カウント（ビット演算）（部位ごと＋部位問わず初絶頂経験）
;　 11：
;　 12：
;　 13：
;　 14：
;　 15：情事目撃回数
;　 16：
;　 17：
;　 18：
;　 19：
;　 20：
;　……以下続刊
;
;
;
;--------------------------------------------------



;--------------------------------------------------
;口上テンプレートreadme
;--------------------------------------------------
;erablue_resort専用口上テンプレート4
;
;・使い方
;XXXXをキャラ番号に置換してください
;0001のようにケタ合わせをする必要はなく、1番のキャラの場合は「1」で置換してください
;そして任意の条件内部の「KSTR:(K++) = 」や「WSTR:(K++) = 」にセリフを追加してください
;
;口上を追加しないコマンドは無記入でも構いませんが、『;』をつけてコメントアウトすると尚良いでしょう
;
;・口上の基本記法
;KSTR:(K++) にセリフを代入した場合、それは表示後に改行されます。PRINTFORMLと同じように使用してください。
;WSTR:(K++) にセリフを代入した場合、それは表示後に改行され、かつ何かの入力があるまで処理を一時待機します。PRINTFORMWと同じように使用してください。
;NSTR:(K++) にセリフを代入した場合、表示後に改行されません。PRINTFORMと同じように使用してください。
;これらはFORM構文に対応しています。文字列変数の中身を表示する際は%で、数値変数の中身を表示する際は{}でくくってください
;
;CSTR:対象キャラ:一人称とCSTR:対象キャラ:二人称という文字列を用意しています。
;この変数を利用することで好感度や陥落状況などで自分やあなたの呼び方を変化させることが出来ます。
;初期値は空っぽなので、利用する場合は「口上側初期パラメータ変更_XXXX」関数内で初期値を設定してください。
;
;・口上の特殊記法
;セリフ内に以下のコードを使うことで特殊表示が可能です。口上作成にご利用下さい。
;（内容の頭に＊が付いているコードは、ダンジョン探索中.ERBやダンジョンハプニング.ERBなど
;　メッセージ欄内に表示されるセリフの場合には使用できません）
;	+-------------------+-------------------------------------------------------------------+
;	|コード             |内容                                                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_BUTTON_           |直後の文字列をボタン化します。                                       |
;	+-------------------+-------------------------------------------------------------------+
;	|_NOBUTTON_         |＊直後の文字列を、文字列の内容に関わらずボタン化せずに表示します。      |
;	+-------------------+-------------------------------------------------------------------+
;	|_CALL_             |直後の文字列を関数名として扱い、CALLします。                          |
;	+-------------------+-------------------------------------------------------------------+
;	|_INPUT_            |INPUTを呼び出します。                                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_INPUTS_           |INPUTSを呼び出します。                                              |
;	+-------------------+-------------------------------------------------------------------+
;	|_COLOR_0xXXXXXX_   |直後の文字列を0xXXXXXXで指定した文字色で表示します                   |
;	+-------------------+-------------------------------------------------------------------+
;	|_-_                |直後の文字列に打ち消し線を引きます                                   |
;	+-------------------+-------------------------------------------------------------------+
;	|_B_                |直後の文字列を太字にします                                          |
;	+-------------------+-------------------------------------------------------------------+
;	|_I_                |直後の文字列を斜体にします                                          |
;	+-------------------+-------------------------------------------------------------------+
;	|_LINE_             |直後の文字列に下線を引きます                                        |
;	+-------------------+-------------------------------------------------------------------+
;	|_FS_X_             |直後の文字列の書式をXに従い変更します                                |
;	|                   |X=1:太字 2:斜体 4:打ち消し線 8:下線。複数指定する場合は加算して下さい |
;	+-------------------+-------------------------------------------------------------------+
;	|_L_                |＊改行します                                                       |
;	|_改行_             |                                                                   |
;	+-------------------+-------------------------------------------------------------------+
;	|_W_                |＊改行し、入力待ち状態にします                                       |
;	+-------------------+-------------------------------------------------------------------+
;	|_WAIT_             |＊改行せず、入力待ち状態にします                                     |
;	+-------------------+-------------------------------------------------------------------+
;	|_FORCEWAIT_        |＊改行せず、スキップ機能でスキップ出来ない入力待ち状態にします         |
;	+-------------------+-------------------------------------------------------------------+
;	|_H_                |ハートマークのアイコンを表示します                                   |
;	+-------------------+-------------------------------------------------------------------+
;	|_A_                |怒りマークのアイコンを表示します                                     |
;	+-------------------+-------------------------------------------------------------------+
;	|_IMAGE_            |直後の文字列で指定した画像を18*18で表示します。絵文字を想定           |
;	+-------------------+-------------------------------------------------------------------+
;	|_呼び名_           |CALLNAME:対象キャラを表示します                                     |
;	|_CALLNAME_         |上記の書式変更コードの影響を受けません                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_一人称_           |CSTR:対象キャラ:一人称を表示します                                   |
;	|_1st_              |上記の書式変更コードの影響を受けません                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_二人称_           |CSTR:対象キャラ:二人称を表示します                                   |
;	|_2nd_              |上記の書式変更コードの影響を受けません                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_主人_             |CALLNAME:MASTERを表示します                                         |
;	|_主人公_           |上記の書式変更コードの影響を受けません                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_DRAWLINE_         |DRAWLINEします。設定に関しては通常のDRAWLINE設定を受け継ぎます。     |
;	+-------------------+-------------------------------------------------------------------+
;また、直後の文字列とは_で区切られた文字列のことを指します
;例えば「KSTR:(K++) = _COLOR_0xFF0000_文章１_文章２_B_文章３_文章４」と記述すると、
;文章１：通常字体、赤色文字
;文章２：通常字体、通常色文字
;文章３：太字体、通常色文字
;文章４：通常字体、通常色文字
;で表示されます
;
;・ダンジョン内でのみ使える口上の特殊記法
;ダンジョン内部の場合、メッセージ欄に文章が表示されます。その場合にのみ使える特殊記法です
;	+-------------------+-------------------------------------------------------------------+
;	|コード             |内容                                                               |
;	+-------------------+-------------------------------------------------------------------+
;	|_PAGE_             |メッセージ欄を一度消去し、新しく表示します。                       |
;	|                   |顔グラや名前表記は維持されます。                                   |
;	+---------------------------------------------------------------------------------------+
;	| NSTR:(K++) = ++++                                                                     |
;	| 切り替え名前:0 = (切替後の名前)                                                       |
;	| 切り替え顔グラリソース:0 = （切替後の顔グラ）                                         |
;	+---------------------------------------------------------------------------------------+
;	| 上の構文は文章内に混ぜたりせずに使用してください。                                    |
;	| メッセージ欄を下に一つ追加して表示する構文です。複数キャラの掛け合いなどを想定。      |
;	| 複数追加する場合は切り替え顔グラリソース:1、切り替え顔グラリソース:2など番号を増やして|
;	| 利用してください。                                                                    |
;	+---------------------------------------------------------------------------------------+
;--------------------------------------------------



