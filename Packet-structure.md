* Packet size: 1-2 bytes (2 byte packet size indicated by 0x80 bit being set, in which case size = 32768 + second byte)
* ObjID: Either 1 byte, or if byte is 0, then after that a thing I will call a WorldsString. 254 is a special destination called "CO"
* Packet type: 1 byte
* Packet data

If the initial ObjID is "CO" (254), Packet data consists of ObjIDs followed by packet data for the packet type.