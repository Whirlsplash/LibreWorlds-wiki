A World. Main object in .world files. Synonyms: "NET.worlds.network.World", "World"

Note that as with all objects, there will first be an object ID, then a class ID, then if the class ID hasn't been seen before (usually the case with Worlds) the class name "NET.worlds.scape.World" (or a synonym).

| Version | Type | Name/Description |
| ---     | ---  | --- |
| All | Version for World | Version for World, 0-13 |
| World >= 1 | Version for SuperRoot | Version for SuperRoot, 0-2 |
| All | String | World name |
| World >= 1, SuperRoot == 1 | MaybeNull | Unknown, discarded |
| All | String | Default room name |
| World <= 6 | String | Server URL, read in an "old" way, might need further description. "UNSHARED" equivalent to null |
| World == 7 | String | Server URL. If null, assumed to a default value, otherwise, World considered to be multiuser |
| World >= 8 | String | Server URL. |
| World == 2 | String | Unknown, discarded |
| World >= 5 | Int | Timeout Age. Note that in versions 8 and below, a Timeout Age of 60000 is converted to 15000 |
| World == 6 or 7 | Boolean | Unknown, discarded |
| World >= 8 | Boolean | Multiuser |
| World >= 10 | Boolean | Courtesy VIP |
| World >= 11 | Boolean | Force Human |
| World >= 12 | Boolean | Has Ad Banner |
| World >= 12 | Integer | Banner Width |
| World >= 12 | Integer | Banner Height |
| World >= 12 | String | Banner URL |
| World == 13 | Boolean | Has Clickable Ad Cube |
| World == 13 | Boolean | Ad Cube Format Is Gif |
| World == 13 | String | Ad Cube Base URL |
| World == 13 | String | Default Ad Cube URL |
| All | Explicit [[NET.worlds.core.Hashtable]] | Hashtable with room name as keys and [[NET.worlds.scape.Room]]s as values |
| World == 4 | Integer | Timeout Age. 60000 and 900000 get read as 15000 |
