# wp_posts

## Description

<details>
<summary><strong>Table Definition</strong></summary>

```sql
CREATE TABLE `wp_posts` (
  `ID` bigint(20) unsigned NOT NULL AUTO_INCREMENT,
  `post_author` bigint(20) unsigned NOT NULL DEFAULT '0',
  `post_date` datetime NOT NULL DEFAULT '0000-00-00 00:00:00',
  `post_date_gmt` datetime NOT NULL DEFAULT '0000-00-00 00:00:00',
  `post_content` longtext COLLATE utf8mb4_unicode_ci NOT NULL,
  `post_title` text COLLATE utf8mb4_unicode_ci NOT NULL,
  `post_excerpt` text COLLATE utf8mb4_unicode_ci NOT NULL,
  `post_status` varchar(20) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT 'publish',
  `comment_status` varchar(20) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT 'open',
  `ping_status` varchar(20) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT 'open',
  `post_password` varchar(255) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT '',
  `post_name` varchar(200) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT '',
  `to_ping` text COLLATE utf8mb4_unicode_ci NOT NULL,
  `pinged` text COLLATE utf8mb4_unicode_ci NOT NULL,
  `post_modified` datetime NOT NULL DEFAULT '0000-00-00 00:00:00',
  `post_modified_gmt` datetime NOT NULL DEFAULT '0000-00-00 00:00:00',
  `post_content_filtered` longtext COLLATE utf8mb4_unicode_ci NOT NULL,
  `post_parent` bigint(20) unsigned NOT NULL DEFAULT '0',
  `guid` varchar(255) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT '',
  `menu_order` int(11) NOT NULL DEFAULT '0',
  `post_type` varchar(20) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT 'post',
  `post_mime_type` varchar(100) COLLATE utf8mb4_unicode_ci NOT NULL DEFAULT '',
  `comment_count` bigint(20) NOT NULL DEFAULT '0',
  PRIMARY KEY (`ID`),
  KEY `post_name` (`post_name`(191)),
  KEY `type_status_date` (`post_type`,`post_status`,`post_date`,`ID`),
  KEY `post_parent` (`post_parent`),
  KEY `post_author` (`post_author`)
) ENGINE=InnoDB AUTO_INCREMENT=2112 DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_unicode_ci
```

</details>

## Columns

| Name                  | Type                | Default             | Nullable | Children | Parents | Comment |
| --------------------- | ------------------- | ------------------- | -------- | -------- | ------- | ------- |
| ID                    | bigint(20) unsigned |                     | false    |          |         |         |
| post_author           | bigint(20) unsigned | 0                   | false    |          |         |         |
| post_date             | datetime            | 0000-00-00 00:00:00 | false    |          |         |         |
| post_date_gmt         | datetime            | 0000-00-00 00:00:00 | false    |          |         |         |
| post_content          | longtext            |                     | false    |          |         |         |
| post_title            | text                |                     | false    |          |         |         |
| post_excerpt          | text                |                     | false    |          |         |         |
| post_status           | varchar(20)         | publish             | false    |          |         |         |
| comment_status        | varchar(20)         | open                | false    |          |         |         |
| ping_status           | varchar(20)         | open                | false    |          |         |         |
| post_password         | varchar(255)        |                     | false    |          |         |         |
| post_name             | varchar(200)        |                     | false    |          |         |         |
| to_ping               | text                |                     | false    |          |         |         |
| pinged                | text                |                     | false    |          |         |         |
| post_modified         | datetime            | 0000-00-00 00:00:00 | false    |          |         |         |
| post_modified_gmt     | datetime            | 0000-00-00 00:00:00 | false    |          |         |         |
| post_content_filtered | longtext            |                     | false    |          |         |         |
| post_parent           | bigint(20) unsigned | 0                   | false    |          |         |         |
| guid                  | varchar(255)        |                     | false    |          |         |         |
| menu_order            | int(11)             | 0                   | false    |          |         |         |
| post_type             | varchar(20)         | post                | false    |          |         |         |
| post_mime_type        | varchar(100)        |                     | false    |          |         |         |
| comment_count         | bigint(20)          | 0                   | false    |          |         |         |

## Constraints

| Name    | Type        | Definition       |
| ------- | ----------- | ---------------- |
| PRIMARY | PRIMARY KEY | PRIMARY KEY (ID) |

## Indexes

| Name             | Definition                                                               |
| ---------------- | ------------------------------------------------------------------------ |
| post_author      | KEY post_author (post_author) USING BTREE                                |
| post_name        | KEY post_name (post_name) USING BTREE                                    |
| post_parent      | KEY post_parent (post_parent) USING BTREE                                |
| type_status_date | KEY type_status_date (post_type, post_status, post_date, ID) USING BTREE |
| PRIMARY          | PRIMARY KEY (ID) USING BTREE                                             |

## Relations

![er](wp_posts.png)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
