## DRAFT

TO paraphrase from the website itself, Cryptopals.com hosts a collection of 48 challenges that demonstrates attacks on real-world crypto.

The incentive is to learn about cryptography by solving a set of challenges rather than learning it from a book or a course. These challenegs takes the concept of learn by doing to another level.

[https://blog.pinboard.in/2013/04/the_matasano_crypto_challenges/]Here is a very well written intro to these challenges.

I've started this blog post as a way to document my progress through the challenges as I go through them.  
So, without further ado I'll start with challenges from set-1.

### Set - 1 : Basics  
#### Challenge - 1 : Convert hex to base64  
The string:  
49276d206b696c6c696e6720796f757220627261696e206c696b65206120706f69736f6e6f7573206d757368726f6f6d  
Should produce:  
SSdtIGtpbGxpbmcgeW91ciBicmFpbiBsaWtlIGEgcG9pc29ub3VzIG11c2hyb29t  
Hmm...how do we tackle this?  
Assuming you already know hex is a base16 (radix16) numeral system. We can move forward with understanding the base64 encoding and what it is used for.  


