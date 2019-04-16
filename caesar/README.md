# Caesar Shifts

## Introduction

Secret codes have existed for about as long as the written word. As soon as mankind could write messages, we wanted to be able to write messages that couldn't be understood by snoops.

One of the oldest (and simplest!) secret codes is known as a _Caesar shift_ - named after Julius Caesar, who used it in his own correspondence.

## The cipher

A Caesar shift cipher consists of choosing a key (between 1 and 25) and shifting the alphabet by that many places, wrapping around at the ends.

For example, with a key of 4, the alphabet becomes:

```
Original: ABCDEFGHIJKLMNOPQRSTUVWXYZ
Encoded:  EFGHIJKLMNOPQRSTUVWXYZABCD
```

The message `ATTACK AT DAWN` would become `EXXEGO EX HEAR`.

When decoding the message, you need to know the original key, and then it's a simple matter of shifting the alphabet the other way.

## Encoding

Write a program that, given an input message and a key, encodes the message using the provided key. Ignore any characters that are not letters.

## Decoding

Extend your program to also allow decoding as an option - the user should be able to choose whether they want to decode or encode.

## Cracking

Add a third mode to your program - one that will attempt to crack some encoded text, perhaps from a file. Your program should attempt to work out the correct key that the text was encoded with - try and come up with some good methods for doing that - and then output what it thinks the decoded text is.

Use the file `ciphertext.txt` as a test for your program's capabilities.