# Lazycode-Minicode
Lazycode is a subset of the US-ASCII character set, which consists of all the characters which can be typed on a US QWERTY layout keyboard without using the Shift key or the CapsLock key. Minicode extends Lazycode with the remaining printable US-ASCII characters.

## Lazycode

Lazycode is called lazy code because all its characters are unshifted, meaning you can type them on a US QWERTY keyboard layout with having to press the Shift key at the same time (or without having to have pressed the CapsLock key first), making it a very lazy code (character set) to type. Specifically, these characters are [in order as the appear on a US QWERTY keyboard layout - from top to bottom - and from left to right]:

the 10 digits

    1 2 3 4 5 6 7 8 9 0

the 26 lowercase letters

    q w e r t y u i o p a s d f g h j k l z x c v b n m

the space character ( ).
     
the following 10 symbols

    - = [ ] \ ; ' , . /
    
and the newline character.

For a total of 48 characters.

An example where Lazycode has been used is the [Confetti](https://github.com/rolancon/confetti) data format language.

### Whitespace

Another characteristic of Lazycode is its visual aspect: every character on the screen should be immediately identifiable (and easily replaceable). Thererefore whitespace (the space and newline) characters have limititations on how they can be combined, otherwise visually it would not be immediately clear which ones are spaces, and which ones newlines. The rules for whitespace are:
- spaces are only used to separate printable characters, they should not appear at the start or end of a document
- there should be at most one space between two printable characters
- the only exception is that one space may appear after a newline (but not before it) when followed by a printable character
- newlines are only used to separate printable characters, they should not appear at the start or end of a document
- the only exceptions is that two newlines may appear next to one another after a printable character when before a printable character, or one space followed by a printable character

It is possible to automate the whitespace normalizaztion of Lazycode documents which do not follow the above whitespace rules. That proces could then also deal with to other whitespace characters as follows:
- a carriage return character before a newline character is dropped (other positions are invalid)
- a tab character is replaced by one space character (whitespace normalization has to be done after the replacement)

## Minicode

