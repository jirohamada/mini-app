# Mini Application DB設計
## usersテーブル
|Column|Type|Option|
|------|----|------|
|name|string|null: false|
|email|stiring|null: false|
|passwprd|string|null: false|
### Association
- has_many :blogs

## blogsテーブル
|Column|Type|Option|
|------|----|------|
|body|text||
|date|datetime||
|user_id|integer|null: false, foreign_key: true|
### Association
- belongs_to :user