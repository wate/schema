# zp_punch_clock

## 概要

<details>
<summary><strong>テーブル定義</strong></summary>

```sql
CREATE TABLE `zp_punch_clock` (
  `id` int(11) unsigned NOT NULL AUTO_INCREMENT,
  `userId` int(11) NOT NULL,
  `minutes` int(11) DEFAULT NULL,
  `hours` int(11) DEFAULT NULL,
  `punchIn` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`,`userId`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci
```

</details>

## カラム一覧

| 名前      | タイプ              | デフォルト値       | Nullable | Extra Definition | 子テーブル      | 親テーブル                 | コメント     |
| ------- | ---------------- | ------------ | -------- | ---------------- | ---------- | --------------------- | -------- |
| id      | int(11) unsigned |              | false    | auto_increment   |            |                       |          |
| userId  | int(11)          |              | false    |                  |            | [zp_user](zp_user.md) |          |
| minutes | int(11)          | NULL         | true     |                  |            |                       |          |
| hours   | int(11)          | NULL         | true     |                  |            |                       |          |
| punchIn | int(11)          | NULL         | true     |                  |            |                       |          |

## 制約一覧

| 名前      | タイプ         | 定義                       |
| ------- | ----------- | ------------------------ |
| PRIMARY | PRIMARY KEY | PRIMARY KEY (id, userId) |

## INDEX一覧

| 名前      | 定義                                   |
| ------- | ------------------------------------ |
| PRIMARY | PRIMARY KEY (id, userId) USING BTREE |

## ER図

![er](zp_punch_clock.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)