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
