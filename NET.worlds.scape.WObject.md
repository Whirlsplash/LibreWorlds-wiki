Most things are subclasses of WObject. WObject is a subclass of [[NET.worlds.scape.Transform]] which is a subclass of [[NET.worlds.scape.SuperRoot]].

| Version | Type | Name/Description |
| --- | --- | --- |
| All | Version for WObject | 0-10 |
| All | Implicit [[Transform|NET.worlds.scape.Transform]] | Transform |
| All | Integer | [[WObject Flags]] |
| 0-1 | MaybeNull | Unknown, discarded |
| All | MaybeNullVector of Explicit WObjects | Contents |
| All | MaybeNullVector of Explicit [[Actions|NET.worlds.scape.Action]] | Actions |
| 1-10 | MaybeNullVector of Explicit [[SuperRoots|NET.worlds.scape.SuperRoot]] | Handlers |