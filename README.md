# TownOfHost-Fun-Json
TOH-Fのニュースなどを簡単に管理できるところ
## ModNews.json
TOH-F内で表示されるニュース情報を定義します。
### 各キーの適用場所
![ModNews.json](https://github.com/user-attachments/assets/a13aeebf-b851-4466-85a2-879c199fe8c7)
(DateにはUTC表記のニュース発表時刻を入力してください)
| キー | 概要 | 記載例 |
|------|------|---|
| Number | ニュースの識別Id<br>最新のJsonNewsのIdに+1したものを使用してください | "2000000" |
| Title | ニュースのタイトル<br>`#00005f`のカラータグを適用すること | "<#00005f>重大なバグの修正</color>" |
| Subtitle | サブタイトル<br>TownOfHost-Fun v.(バージョン)のように記載すること | "TownOfHost-Fun v.3.0.0.0.β" |
| Short | ニュース一覧タブに表示されるテキスト<br>`#00005f`のカラータグを適用し、<br>(開発者マーク)TOH-F v.(バージョン)のように記載すること | "<#00005f><b>★</b>TOH-F v.3.0.0.0</color>" |
| Body | ニュースの内容 | "重大なバグを修正しました。\n・部屋を立てることが出来ないバグ" |
| Date | ニュース発表日時(UTC表記) | "2025-01-01T00:00:00Z" |
#### 例
```
{
  "Number": "2000000",
  "Title": "てすと",
  "Subtitle": "～てすと～",
  "Short": "-てすと-",
  "Body": "jsonNewsのテスト。",
  "Date": "2020-01-01T00:00:00Z"
}
```
