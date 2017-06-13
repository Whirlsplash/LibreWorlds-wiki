Data in Persister format does not mark itself to indicate their types, the types are assumed by the deserialization code. That is, a Portal being read in knows when to expect a boolean, a string, and an integer, for example. Without knowing what a Portal wants to read, it is not possible to determine where the next item begins.

# Primitive data types

Worlds generally uses the format described by [Java's DataInput](https://docs.oracle.com/javase/7/docs/api/java/io/DataInput.html).

* String: Starts with a byte, where 0x01 means the string is null (and the next byte is for the next item) and 0x00 means non-null. If non-null, next 2 bytes are the length in number of bytes (big-endian). Following is the actual string data, in modified UTF-8. (The bytes after the non-null indicator are merely read by DataInput).
* Boolean: 1 byte, 0x00 for false 0x01 for true.
