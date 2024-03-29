# ConfigurationFiles

## 概要

<details>
<summary><strong>テーブル定義</strong></summary>

```sql
CREATE TABLE `ConfigurationFiles` (
  `Name` varchar(64) NOT NULL,
  `Data` mediumtext DEFAULT NULL,
  `CreateAt` bigint(20) NOT NULL,
  `UpdateAt` bigint(20) NOT NULL,
  PRIMARY KEY (`Name`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4
```

</details>

## カラム一覧

| 名前       | タイプ         | デフォルト値       | NULL許可   | 子テーブル      | 親テーブル      | コメント     |
| -------- | ----------- | ------------ | -------- | ---------- | ---------- | -------- |
| Name     | varchar(64) |              | false    |            |            |          |
| Data     | mediumtext  | NULL         | true     |            |            |          |
| CreateAt | bigint(20)  |              | false    |            |            |          |
| UpdateAt | bigint(20)  |              | false    |            |            |          |

## 制約一覧

| 名前      | タイプ         | 定義                 |
| ------- | ----------- | ------------------ |
| PRIMARY | PRIMARY KEY | PRIMARY KEY (Name) |

## INDEX一覧

| 名前      | 定義                             |
| ------- | ------------------------------ |
| PRIMARY | PRIMARY KEY (Name) USING BTREE |

## ER図

![er](ConfigurationFiles.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
