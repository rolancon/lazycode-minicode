# Lazycode-Minicode
Lazycode is a subset of the [US-ASCII](https://en.wikipedia.org/wiki/ASCII) character set: it consists of all the characters which can be typed on a [US-QWERTY](https://en.wikipedia.org/wiki/QWERTY) layout keyboard without using the Shift key or the CapsLock key. Minicode extends Lazycode with the remaining printable ASCII characters.

## Lazycode

Lazycode is called lazy code because all its characters are unshifted, meaning you can type them on a QWERTY keyboard layout with having to press the Shift key at the same time (or without having to have pressed the CapsLock key first), making it a very lazy code (character set) to type. Specifically, these characters are [in order as the appear on a QWERTY keyboard layout - from top to bottom - and from left to right]:

the 10 digits

    1 2 3 4 5 6 7 8 9 0

the 26 lowercase letters

    q w e r t y u i o p a s d f g h j k l z x c v b n m

the space character
     
the following 10 symbols

    - = [ ] \ ; ' , . /
    
and the newline character.

For a total of 48 characters.

Lazycode is especially suitable for simple programming codes, which could be easily created and edited in a text editor, and processed with other programs. An example where Lazycode has been used is the [Confetti](https://github.com/rolancon/confetti) data format language.

### Whitespace

Another characteristic of Lazycode is its visual aspect: every character on the screen should be immediately identifiable (and easily replaceable). Thererefore the whitespace (space and newline) characters have limititations on how they can be combined, otherwise visually it would not be immediately clear which ones are spaces, and which ones newlines. The rules for whitespace are:
- spaces are only used to separate printable characters, they should not appear at the start or end of a document
- there should be at most one space between two printable characters
- newlines are only used to separate printable characters, they should not appear at the start or end of a document
- the only exception is that two newlines may appear next to one another in between printable characters

It is possible to automate the whitespace normalizaztion of Lazycode documents which do not follow the above whitespace rules. That proces could then also deal with two other whitespace characters, which commonly appear when creating or editing a document in a text editor, as follows:
- a carriage return character before a newline character is dropped (other positions are invalid)
- a tab character is replaced by one space character (whitespace normalization has to be done after the replacement)

## Minicode

