`NET.worlds.scape.Room` is a subtype of [[NET.worlds.scape.WObject]] which is a subtype of [[NET.worlds.scape.Transform]] which is a subtype of [[NET.worlds.scape.SuperRoot]].

| Version | Type | Name/Description |
| --- | --- | --- |
| All | Version for Room | 0-7 |
| All | Implicit [[WObject|NET.worlds.scape.WObject]] | Includes room contents, actions, event handlers, and room name for non-0 version |
| 0 | String | Room name |
| 0-1 | Explicit Object | Unknown, discarded |
| All | Boolean | Null indicator: False = Skip next entry |
| All | Integer | Sky Color |
| All | Boolean | Null indicator: False = Skip next entry |
| All | Integer | Ground Color |
| 0-3 | MaybeNull  Unknown, discarded |
