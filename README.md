## 名称（Title）
万葉（Mangyoh）
<br>
## 開発環境（Development environment）
* ruby 2.6.3p62 (2019-04-16 revision 67580) [x86_64-darwin18]
* Rails 5.2.3
* psql (PostgreSQL) 11.5
<br>
## テーブル構成（Database Table Info）
|User|||
|:-:|:-:|:-:|
|PK|id||
||name|string|
<br>

|Task|||
|:-:|:-:|:-:|
|PK|id||
|FK|user_id|integer|
||title<br>content<br>limit<br>priority<br>status|string<br>text<br>datetime<br>integer<br>integer|
<br>

|Tagging|||
|:-:|:-:|:-:|
|PK|id||
|FK|task_id|integer|
|FK|tag_id|integer|
<br>

|Tag|||
|:-:|:-:|:-:|
|PK|id||
||title|string|