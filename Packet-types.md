* 0x01 = LONGLOC = Used for long movement and z-coordinate movement.
* 0x02 = STATE?
* 0x03 = PROP = Old-style property list, can be sent or received.
* 0x04 = SHORTLOC = Movement deltas, not along z-axis.
* 0x05 = ROOMCHNG = Indication of user changing rooms, includes new location within room
* 0x06 = SESSIONINIT = Used by client to log in to a server, and server to acknowledge and provider more information. Uses old-style property list
* 0x07 = SESSIONEXIT = Used by client to log off of a server, and server to acknowledge. Uses old-style property list.
* 0x08 = APPINIT = Usage unknown, does not seem to be sent by client. Modifies a state machine upon being received by client. Uses new-style property list.
* 0x0A = PROPREQ = 
