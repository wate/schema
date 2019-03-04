# entries

## Description

<details>
<summary><strong>Table Definition</strong></summary>

```sql
CREATE TABLE `entries` (
  `guid` varchar(32) NOT NULL,
  `date` datetime NOT NULL DEFAULT '1970-01-01 00:00:00',
  `date_entered` datetime DEFAULT '1970-01-01 00:00:00',
  `description` varchar(2048) DEFAULT NULL,
  `action` varchar(2048) DEFAULT NULL,
  `notes` varchar(2048) DEFAULT NULL,
  `quantity_num` bigint(20) DEFAULT NULL,
  `quantity_denom` bigint(20) DEFAULT NULL,
  `i_acct` varchar(32) DEFAULT NULL,
  `i_price_num` bigint(20) DEFAULT NULL,
  `i_price_denom` bigint(20) DEFAULT NULL,
  `i_discount_num` bigint(20) DEFAULT NULL,
  `i_discount_denom` bigint(20) DEFAULT NULL,
  `invoice` varchar(32) DEFAULT NULL,
  `i_disc_type` varchar(2048) DEFAULT NULL,
  `i_disc_how` varchar(2048) DEFAULT NULL,
  `i_taxable` int(11) DEFAULT NULL,
  `i_taxincluded` int(11) DEFAULT NULL,
  `i_taxtable` varchar(32) DEFAULT NULL,
  `b_acct` varchar(32) DEFAULT NULL,
  `b_price_num` bigint(20) DEFAULT NULL,
  `b_price_denom` bigint(20) DEFAULT NULL,
  `bill` varchar(32) DEFAULT NULL,
  `b_taxable` int(11) DEFAULT NULL,
  `b_taxincluded` int(11) DEFAULT NULL,
  `b_taxtable` varchar(32) DEFAULT NULL,
  `b_paytype` int(11) DEFAULT NULL,
  `billable` int(11) DEFAULT NULL,
  `billto_type` int(11) DEFAULT NULL,
  `billto_guid` varchar(32) DEFAULT NULL,
  `order_guid` varchar(32) DEFAULT NULL,
  PRIMARY KEY (`guid`)
) ENGINE=InnoDB DEFAULT CHARSET=utf8
```

</details>

## Columns

| Name             | Type          | Default             | Nullable | Children | Parents | Comment |
| ---------------- | ------------- | ------------------- | -------- | -------- | ------- | ------- |
| guid             | varchar(32)   |                     | false    |          |         |         |
| date             | datetime      | 1970-01-01 00:00:00 | false    |          |         |         |
| date_entered     | datetime      | 1970-01-01 00:00:00 | true     |          |         |         |
| description      | varchar(2048) |                     | true     |          |         |         |
| action           | varchar(2048) |                     | true     |          |         |         |
| notes            | varchar(2048) |                     | true     |          |         |         |
| quantity_num     | bigint(20)    |                     | true     |          |         |         |
| quantity_denom   | bigint(20)    |                     | true     |          |         |         |
| i_acct           | varchar(32)   |                     | true     |          |         |         |
| i_price_num      | bigint(20)    |                     | true     |          |         |         |
| i_price_denom    | bigint(20)    |                     | true     |          |         |         |
| i_discount_num   | bigint(20)    |                     | true     |          |         |         |
| i_discount_denom | bigint(20)    |                     | true     |          |         |         |
| invoice          | varchar(32)   |                     | true     |          |         |         |
| i_disc_type      | varchar(2048) |                     | true     |          |         |         |
| i_disc_how       | varchar(2048) |                     | true     |          |         |         |
| i_taxable        | int(11)       |                     | true     |          |         |         |
| i_taxincluded    | int(11)       |                     | true     |          |         |         |
| i_taxtable       | varchar(32)   |                     | true     |          |         |         |
| b_acct           | varchar(32)   |                     | true     |          |         |         |
| b_price_num      | bigint(20)    |                     | true     |          |         |         |
| b_price_denom    | bigint(20)    |                     | true     |          |         |         |
| bill             | varchar(32)   |                     | true     |          |         |         |
| b_taxable        | int(11)       |                     | true     |          |         |         |
| b_taxincluded    | int(11)       |                     | true     |          |         |         |
| b_taxtable       | varchar(32)   |                     | true     |          |         |         |
| b_paytype        | int(11)       |                     | true     |          |         |         |
| billable         | int(11)       |                     | true     |          |         |         |
| billto_type      | int(11)       |                     | true     |          |         |         |
| billto_guid      | varchar(32)   |                     | true     |          |         |         |
| order_guid       | varchar(32)   |                     | true     |          |         |         |

## Constraints

| Name    | Type        | Definition         |
| ------- | ----------- | ------------------ |
| PRIMARY | PRIMARY KEY | PRIMARY KEY (guid) |

## Indexes

| Name    | Definition                     |
| ------- | ------------------------------ |
| PRIMARY | PRIMARY KEY (guid) USING BTREE |

## Relations

![er](entries.png)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
