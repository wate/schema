# gnclock

## 概要

<details>
<summary><strong>テーブル定義</strong></summary>

```sql
CREATE TABLE `gnclock` (
  `Hostname` varchar(255) DEFAULT NULL,
  `PID` int(11) DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_general_ci
```

</details>

## カラム一覧

| 名前       | タイプ          | デフォルト値       | NULL許可   | 子テーブル      | 親テーブル      | コメント     |
| -------- | ------------ | ------------ | -------- | ---------- | ---------- | -------- |
| Hostname | varchar(255) | NULL         | true     |            |            |          |
| PID      | int(11)      | NULL         | true     |            |            |          |

## ER図

![er](gnclock.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
