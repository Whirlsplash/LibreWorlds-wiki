A World. Main object in .world files. Synonyms: "NET.worlds.network.World", "World"

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
| World >= 5 | Int | Timeout Age |
| World == 6 or 7 | Boolean | Unknown, discarded |
| 
