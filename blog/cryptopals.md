## DRAFT

To paraphrase from the website itself, Cryptopals.com hosts a collection of 48 challenges that demonstrates attacks on real-world crypto.

The incentive is to learn about cryptography by solving a set of challenges rather than learning it from a book or a course. These challenegs takes the concept of learn by doing to another level.

[Here](https://blog.pinboard.in/2013/04/the_matasano_crypto_challenges/) is a very well written intro to these challenges.

I've started this blog post as a way to document my progress through the challenges as I go through them.  
So, without further ado I'll start with challenges from set-1.

### Set - 1 : Basics  
#### Challenge - 1 : Convert hex to base64  
The string:  
'''49276d206b696c6c696e6720796f757220627261696e206c696b65206120706f69736f6e6f7573206d757368726f6f6d'''  
Should produce:  
'''SSdtIGtpbGxpbmcgeW91ciBicmFpbiBsaWtlIGEgcG9pc29ub3VzIG11c2hyb29t'''

Hmm...how do we tackle this?  
Assuming you already know that hex is a radix16 numeral system. We can overview Base64 encoding and what it is used for.

##### Base64:
Foremost challenge while transmitting raw binary data across networks is that, some of it can be misinterpreted as commands or part of the protocol by the devices like router or modem. In order to avoid that binary data is encoded using Base64 representation in such a manner that the resulting data will contain any one of 64 ASCII characters which can be reliably transferred across systems.
E.g. 
- The string '''Man''' (binary: '''010011010110000101101110''') can be converted to Base64 by grouping 6 bits together from left to right and converting them to corresponding ASCII characters.
- '''=''' is used as a padding characters to make the last encoded block contain four Base64 characters.

[Wikipedia](https://en.wikipedia.org/wiki/Base64) has an informative article on Base64 representation which explains things in a further depth.  

##### Code:  
*Rule: Always operate on raw bytes, never on encoded strings. Only use hex and base64 for pretty-printing.*  

'''Python
Code goes here!

'''


