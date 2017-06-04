* 0x01 = LONGLOC = Used for long movement and z-coordinate movement.
* 0x02 = STATE?
* 0x03 = PROP = Old-style property list, can be sent or received.
* 0x04 = SHORTLOC = Movement deltas, not along z-axis.
* 0x05 = ROOMCHNG = Indication of user changing rooms, includes new location within room
* 0x06 = SESSINIT = Used by client to log in to a server, and server to acknowledge and provider more information. Uses old-style property list
* 0x07 = SESSEXIT = Used by client to log off of a server, and server to acknowledge. Uses old-style property list.
* 0x08 = APPINIT = Usage unknown, does not seem to be sent by client. Modifies a state machine upon being received by client. Uses new-style property list.
* 0x0A = PROPREQ = Used by client to request properties. May include a list of properties to request, but that functionality seems to be unused.
* 0x0B = DISAPPR = Used by server to indicate a Drone should disappear.
* 0x0C = APPRACTR = Used by server to indicate a Drone should appear at a room (indicated with a u16), at x, y, z, dir.
* 0x0D = REGOBJID = Used by server to associate a long Object ID with a short Object ID, to save bandwidth. These associations seem to be per connection. The object ID in the packet frame is not used for this, and is 0xFF (target connection).
* 0x0E = TEXT = Used for chat. Includes an ObjID in the data itself, the ObjID in the packet frame is ignored.
* 0x0F = PROPSET = Usually sent from client to server, although there is support for it to be sent server to client as a NOOP. This packet indicates a property change (e.g. avatar or sleep). It also can be sent for shared state, which can affect the objid it gets sent with. The packet format includes a string marked as "fromUser" but usually empty.
* 0x10 = PROPUPD = Sent from server to client with a new-style property list to update properties on the given ObjID.
* 0x11 = WHISPER = Whispering. Includes a sender ID, and uses frame's ObjID for destination.
* 0x12 = TELEPORT = Sent to server for teleporting, sent from server for drones teleporting (includes entering and leaving).
* 0x14 = ROOMIDRQ = Sent to server to request numeric room ID for room name (e.g. "GroundZero#ChatElevator\<dimension-1\>").
* 0x15 = ROOMID = Reply from sever to associate room name with numeric room ID.
* 0x16 = SUBSCRIB (subscribe room) = Subscribe to a room (with numeric room ID) at a location and a distance.
* 0x17 = UNSUBSCR = Unsubscribe from a room.
* 0x18 = SUB-DIST = Subscribe to a room at a distance? Mostly after having moved, but I'm unclear on this. It is in use, as is SUBSCRIB.
* 0x19 = REDIRECT = No-op.
* 0x1A = REDIRID = Sent from server to client to reassign room ID\<-\>room name mapping and point to a different RoomServer?
* 0x1B = FINGREQ = Unused.
* 0x1C = FINGREP = Unused.
