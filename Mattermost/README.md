# Database Schema

## テーブル一覧

| 名前                                                        | カラム一覧      | コメント     | タイプ        |
| --------------------------------------------------------- | ---------- | -------- | ---------- |
| [Audits](Audits.md)                                       | 7          |          | BASE TABLE |
| [Bots](Bots.md)                                           | 7          |          | BASE TABLE |
| [ChannelMemberHistory](ChannelMemberHistory.md)           | 4          |          | BASE TABLE |
| [ChannelMembers](ChannelMembers.md)                       | 13         |          | BASE TABLE |
| [Channels](Channels.md)                                   | 19         |          | BASE TABLE |
| [ClusterDiscovery](ClusterDiscovery.md)                   | 8          |          | BASE TABLE |
| [Commands](Commands.md)                                   | 18         |          | BASE TABLE |
| [CommandWebhooks](CommandWebhooks.md)                     | 7          |          | BASE TABLE |
| [Compliances](Compliances.md)                             | 11         |          | BASE TABLE |
| [ConfigurationFiles](ConfigurationFiles.md)               | 4          |          | BASE TABLE |
| [Configurations](Configurations.md)                       | 5          |          | BASE TABLE |
| [db_config_migrations](db_config_migrations.md)           | 2          |          | BASE TABLE |
| [db_lock](db_lock.md)                                     | 2          |          | BASE TABLE |
| [db_migrations](db_migrations.md)                         | 2          |          | BASE TABLE |
| [Emoji](Emoji.md)                                         | 6          |          | BASE TABLE |
| [FileInfo](FileInfo.md)                                   | 20         |          | BASE TABLE |
| [GroupChannels](GroupChannels.md)                         | 7          |          | BASE TABLE |
| [GroupMembers](GroupMembers.md)                           | 4          |          | BASE TABLE |
| [GroupTeams](GroupTeams.md)                               | 7          |          | BASE TABLE |
| [IncomingWebhooks](IncomingWebhooks.md)                   | 12         |          | BASE TABLE |
| [Jobs](Jobs.md)                                           | 9          |          | BASE TABLE |
| [Licenses](Licenses.md)                                   | 3          |          | BASE TABLE |
| [LinkMetadata](LinkMetadata.md)                           | 5          |          | BASE TABLE |
| [NotifyAdmin](NotifyAdmin.md)                             | 5          |          | BASE TABLE |
| [OAuthAccessData](OAuthAccessData.md)                     | 7          |          | BASE TABLE |
| [OAuthApps](OAuthApps.md)                                 | 12         |          | BASE TABLE |
| [OAuthAuthData](OAuthAuthData.md)                         | 8          |          | BASE TABLE |
| [OutgoingWebhooks](OutgoingWebhooks.md)                   | 16         |          | BASE TABLE |
| [PluginKeyValueStore](PluginKeyValueStore.md)             | 4          |          | BASE TABLE |
| [PostReminders](PostReminders.md)                         | 3          |          | BASE TABLE |
| [Posts](Posts.md)                                         | 18         |          | BASE TABLE |
| [Preferences](Preferences.md)                             | 4          |          | BASE TABLE |
| [ProductNoticeViewState](ProductNoticeViewState.md)       | 4          |          | BASE TABLE |
| [PublicChannels](PublicChannels.md)                       | 7          |          | BASE TABLE |
| [Reactions](Reactions.md)                                 | 8          |          | BASE TABLE |
| [RecentSearches](RecentSearches.md)                       | 4          |          | BASE TABLE |
| [RemoteClusters](RemoteClusters.md)                       | 11         |          | BASE TABLE |
| [RetentionPolicies](RetentionPolicies.md)                 | 3          |          | BASE TABLE |
| [RetentionPoliciesChannels](RetentionPoliciesChannels.md) | 2          |          | BASE TABLE |
| [RetentionPoliciesTeams](RetentionPoliciesTeams.md)       | 2          |          | BASE TABLE |
| [Roles](Roles.md)                                         | 10         |          | BASE TABLE |
| [Schemes](Schemes.md)                                     | 18         |          | BASE TABLE |
| [Sessions](Sessions.md)                                   | 11         |          | BASE TABLE |
| [SharedChannelAttachments](SharedChannelAttachments.md)   | 5          |          | BASE TABLE |
| [SharedChannelRemotes](SharedChannelRemotes.md)           | 10         |          | BASE TABLE |
| [SharedChannels](SharedChannels.md)                       | 12         |          | BASE TABLE |
| [SharedChannelUsers](SharedChannelUsers.md)               | 6          |          | BASE TABLE |
| [SidebarCategories](SidebarCategories.md)                 | 9          |          | BASE TABLE |
| [SidebarChannels](SidebarChannels.md)                     | 4          |          | BASE TABLE |
| [Status](Status.md)                                       | 6          |          | BASE TABLE |
| [Systems](Systems.md)                                     | 2          |          | BASE TABLE |
| [TeamMembers](TeamMembers.md)                             | 8          |          | BASE TABLE |
| [Teams](Teams.md)                                         | 17         |          | BASE TABLE |
| [TermsOfService](TermsOfService.md)                       | 4          |          | BASE TABLE |
| [ThreadMemberships](ThreadMemberships.md)                 | 6          |          | BASE TABLE |
| [Threads](Threads.md)                                     | 6          |          | BASE TABLE |
| [Tokens](Tokens.md)                                       | 4          |          | BASE TABLE |
| [UploadSessions](UploadSessions.md)                       | 11         |          | BASE TABLE |
| [UserAccessTokens](UserAccessTokens.md)                   | 5          |          | BASE TABLE |
| [UserGroups](UserGroups.md)                               | 10         |          | BASE TABLE |
| [Users](Users.md)                                         | 26         |          | BASE TABLE |
| [UserTermsOfService](UserTermsOfService.md)               | 3          |          | BASE TABLE |

## ER図

![er](schema.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
