## PROJECT ##

* ID: **B**encode!**P**ARSER
* Contact: git@schepsen.eu

## USAGE ##

To use the **B**encode!**P**ARSER you need to add the header file in your project

## SPECIFICATION ##

* Bencode http://www.bittorrent.org/beps/bep_0003.html

## EXAMPLES ##

std::string src("d3:bar4:spam3:fooi42ee");

```
BencodeNode root
(
    BDecoder(src).decode()
);
```
encodes to a BencodeNode-Structure
```
{ "bar" : "spam", "foo" : 42 }

```
## CHANGELOG ##

### Bencode!PARSER 1.1, updated @ 2016-03-22 ###

* Added the function encode() BEncodes a BencodeNode

### Bencode!PARSER 1.0, updated @ 2016-03-02 ###

* Added the function toString() prints formatted code after its decoding

### Bencode!PARSER 1.0, updated @ 2016-03-01 ###

* Initial release
