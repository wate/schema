# zp_calendar

## 概要

<details>
<summary><strong>テーブル定義</strong></summary>

```sql
CREATE TABLE `zp_calendar` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `userId` int(11) DEFAULT NULL,
  `dateFrom` datetime DEFAULT NULL,
  `dateTo` datetime DEFAULT NULL,
  `description` text DEFAULT NULL,
  `kind` varchar(255) DEFAULT NULL,
  `allDay` varchar(10) DEFAULT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci
```

</details>

## カラム一覧

| 名前          | タイプ          | デフォルト値       | Nullable | Extra Definition | 子テーブル      | 親テーブル                 | コメント     |
| ----------- | ------------ | ------------ | -------- | ---------------- | ---------- | --------------------- | -------- |
| id          | int(11)      |              | false    | auto_increment   |            |                       |          |
| userId      | int(11)      | NULL         | true     |                  |            | [zp_user](zp_user.md) |          |
| dateFrom    | datetime     | NULL         | true     |                  |            |                       |          |
| dateTo      | datetime     | NULL         | true     |                  |            |                       |          |
| description | text         | NULL         | true     |                  |            |                       |          |
| kind        | varchar(255) | NULL         | true     |                  |            |                       |          |
| allDay      | varchar(10)  | NULL         | true     |                  |            |                       |          |

## 制約一覧

| 名前      | タイプ         | 定義               |
| ------- | ----------- | ---------------- |
| PRIMARY | PRIMARY KEY | PRIMARY KEY (id) |

## INDEX一覧

| 名前      | 定義                           |
| ------- | ---------------------------- |
| PRIMARY | PRIMARY KEY (id) USING BTREE |

## ER図

![er](zp_calendar.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
