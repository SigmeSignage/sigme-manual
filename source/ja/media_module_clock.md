<!--toc=widgets-->

# 時計

時計ウィジェットは、**アナログ時計**、*フリップ時計**、*デジタル時計**を表示するために使用することができます。

## ウィジェッを追加

[ウィジェット](layouts_widgets.html)ツールバーの**時計**をクリックし、追加またはドラッグ＆ドロップで追加します。 
![Clock Widget](img\v2_media_clock_widget.png)

追加すると、設定オプションがプロパティパネルに表示されます。

- 識別しやすいように **名前** を記入してください。
- 必要であれば、デフォルトの**期間**をオーバーライドするよう選択します。

### 外観

ドロップダウンメニューで、表示する時計の種類を選択します。

![Clock Appearance](img\v3.1_media_clock_appearance.png)

- **アナログ時計**は、伝統的な時計の文字盤で、ライトとダークのテーマ（ブラックまたはホワイトの文字盤）が用意されています。
- **デジタル時計**には、フォーマットを入力するための**エディタ**タブが追加されています。

テキストまたはHTMLをボックスに入力するか、ビジュアルエディタをオンにして編集アイコンをクリックすると、インラインエディタにアクセスできます。

![Digital Editor](img/v3.1_media_clock_editor.png)

エディタでフォント、サイズ、カラーを選択し、**スニペット**を使用して利用可能なマージフィールドを含めることができます。

{tip}
日付/時刻フォーマットの詳細については、ページ下部のセクションをご覧ください
{/tip}


- **フリップ時計** 時、分、秒（オプション）が経過するごとに「めくり」がアニメーションで表示されるプリフォーマットな時計です。

{tip}
**フリップクロック**には、時間単位、分単位、日単位の**カウンタ**オプションがあり、指定した日付/時刻からカウントダウンを実行することができます!
{/tip}

## アクション

このウィジェットにはアクションを付けることができます。詳しくは[インタラクティブアクション](layouts_interactive_actions.html)のページを参照してください。

## 時間の書式設定

テンプレート領域の角括弧[]の間にある”トークン”を指定することで時刻をフォーマットできます。


| タイトル                      | トークン   | 出力                                 |
| -------------------------- | ------- | -------------------------------------- |
| 月                     | M       | 1 2 ... 11 12                          |
|                            | Mo      | 1st 2nd ... 11th 12th                  |
|                            | MM      | 01 02 ... 11 12                        |
|                            | MMM     | Jan Feb ... Nov Dec                    |
|                            | MMMM    | 1月 2月 ... 11月 12月 |
| 四半期                    | Q       | 1 2 3 4                                |
| 月の日付               | D       | 1 2 ... 30 31                          |
|                            | Do      | 1st 2nd ... 30th 31st                  |
|                            | DD      | 01 02 ... 30 31                        |
| 年の日付                | DDD     | 1 2 ... 364 365                        |
|                            | DDDo    | 1st 2nd ... 364th 365th                |
|                            | DDDD    | 001 002 ... 364 365                    |
| 曜日                | d       | 0 1 ... 5 6                            |
|                            | do      | 0th 1st ... 5th 6th                    |
|                            | dd      | 日 月 ... 金 土                        |
|                            | ddd     | 日曜 月曜 ... 金曜 土曜                  |
|                            | dddd    | 日曜日 月曜日 ... 金曜日 土曜日     |
| 週の日付 (Locale)       | e       | 0 1 ... 5 6                            |
| 週の日付 (ISO)          | E       | 1 2 ... 6 7                            |
| 年の週               | w       | 1 2 ... 52 53                          |
|                            | wo      | 1st 2nd ... 52nd 53rd                  |
|                            | ww      | 01 02 ... 52 53                        |
| 年の週(ISO)         | W       | 1 2 ... 52 53                          |
|                            | Wo      | 1st 2nd ... 52nd 53rd                  |
|                            | WW      | 01 02 ... 52 53                        |
| 年                       | YY      | 70 71 ... 29 30                        |
|                            | YYYY    | 1970 1971 ... 2029 2030                |
| 週の年                  | gg      | 70 71 ... 29 30                        |
|                            | gggg    | 1970 1971 ... 2029 2030                |
| 週の年 (ISO)            | GG      | 70 71 ... 29 30                        |
|                            | GGGG    | 1970 1971 ... 2029 2030                |
| AM/PM                      | A       | AM PM                                  |
|                            | a       | am pm                                  |
| 時                       | H       | 0 1 ... 22 23                          |
|                            | HH      | 00 01 ... 22 23                        |
|                            | h       | 1 2 ... 11 12                          |
|                            | hh      | 01 02 ... 11 12                        |
| 分                     | m       | 0 1 ... 58 59                          |
|                            | mm      | 00 01 ... 58 59                        |
| 秒                     | s       | 0 1 ... 58 59                          |
|                            | ss      | 00 01 ... 58 59                        |
| 小数秒          | S       | 0 1 ... 8 9                            |
|                            | SS      | 0 1 ... 98 99                          |
|                            | SSS     | 0 1 ... 998 999                        |
| タイムゾーン                   | z or zz | EST CST ... MST PST                    |
|                            | Z       | -07:00 -06:00 ... +06:00 +07:00        |
|                            | ZZ      | -0700 -0600 ... +0600 +0700            |
| Unixタイムスタンプ             | X       | 1360013296                             |
| Unixミリ秒タイムスタンプ | x       | 1360013296123                          |


