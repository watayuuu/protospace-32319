# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

# テーブル設計

## usersテーブル
| Column     | Type       | Options     |
| ---------- | ---------- | ----------- |
| email      | string     | null: false |
| password   | references | null: false |
| name       | string     | null: false |
| profile    | text       | null: false |
| occupation | text       | null: false |
| position   | text       | null: false |

## commentsテーブル
| Column     | Type       | Options     |
| ---------- | ---------- | ----------- |
| text       | string     | null: false |
| user       | references |             |
| prototype  | references |             |

## prototypesテーブル
| Column     | Type       | Options     |
| ---------- | ---------- | ----------- |
| title      | string     | null: false |
| catch_copy | text       | null: false |
| concept    | text       | null: false |
| image      |            |             |
| user       | references |             |



