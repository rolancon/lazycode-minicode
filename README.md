# Lazycode-Minicode
Lazycode is a subset of the [US-ASCII](https://en.wikipedia.org/wiki/ASCII) character set: it consists of all the characters which can be typed on a [US-QWERTY](https://en.wikipedia.org/wiki/QWERTY) layout keyboard without using the Shift key or the CapsLock key. Minicode extends Lazycode with the remaining printable ASCII characters.

## Lazycode

Lazycode is called lazy code because all its characters are unshifted, meaning you can type them on a QWERTY keyboard layout with having to press the Shift key at the same time (or without having to have pressed the CapsLock key first), making it a very lazy code (character set) to type. Specifically, these characters are [in order as the appear on a QWERTY keyboard layout - from top to bottom - and from left to right]:

the 10 digits

    1 2 3 4 5 6 7 8 9 0

the 26 lowercase letters

    q w e r t y u i o p a s d f g h j k l z x c v b n m
    
the following 10 symbols

    - = [ ] \ ; ' , . /
    
the space character and the newline character,
for a total of 48 characters.

The digits, letters, and symbols are called printable characters, because they are visible on screen.

Lazycode is especially suitable for basic programming codes, which could be easily created and edited in a text editor, and processed with other programs. An example where Lazycode has been used is the simple [Confetti](https://github.com/rolancon/confetti) data format language.

### Whitespace

Another characteristic of Lazycode is its visual aspect: every character on the screen should be immediately identifiable (and easily replaceable). Thererefore the whitespace (space and newline) characters have limititations on how they can be combined, otherwise visually it would not be immediately clear which ones are spaces, and which ones newlines. The rules for whitespace are:
- spaces are only used to separate two printable characters, they should not appear at the start or end of a document
- there should be at most one space between two printable characters
- newlines are only used to separate printable characters, they should not appear at the start or end of a document
- there should be at most one or two newlines in between printable characters

It is possible to automate the whitespace normalizaztion of Lazycode documents which do not follow the above whitespace rules. That proces could then also deal with two other whitespace characters, which commonly appear when creating or editing a document in a text editor, as follows:
- a carriage return character before a newline character is dropped (other positions are invalid)
- a tab character is replaced by one space character (whitespace normalization has to be done after the replacement)

## Minicode

Minicode is called mini code as a pun on Unicode: whereas Unicode contains all possible characters known to humankind, Minicode is the bare minimum character set from the ASCII subset of Unicode. It extends Lazycode with the remaining printable ASCII characters that appear on a QWERTY layout keyboard. The extended character set consists of [following the keyboard layout]:

the 26 uppercase letters

    Q W E R T Y U I O P A S D F G H J K L Z X C V B N M

the 22 symbols

    ~ ` ! @ # $ % ^ & * ( ) _ + { } | : " < > ?

for a total of 48 characters. The combined total number of characters in Minicode (since it extends Lazycode) is 96.

Minicode is more suited for extended programming codes, which can still be easily created and edited in a text editor, and processed with other programs. It can also be used to write texts. An example where Minicode has been used is in the [string datatype](https://github.com/rolancon/confetti#types) of Confetti.

The whitespace normalization rules of Lazycode might be relaxed if that suits the purpose of a particular usage of Minicode.
