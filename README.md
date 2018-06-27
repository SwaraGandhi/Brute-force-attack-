# Brute-force-attack-

Imagine a lock on a door without a key. To open the door you could simply pick up something and start smashing the lock (and hope it opens)
or you could brute force the lock by using lock picks and picking the individual pins in the chamber.

An example of a simple brute force where we attempt to discover a hidden two digit number is below. Here we loop around all possible 
numbers from ‘0’ and stop when we hit the correct answer.

> Example

Hidden Number: 18

Brute Force Attempts: 00, 01, 02, 03, 04, 05, 06, 07, 08, 09, 10, 11, 12, 13, 14, 15, 16, 17, 18

Answer: 18

> Program description :

Brute force method that will guess numbers (string.digits) and lower case letters (string.ascii_lowercase). 

Can use itertools.product with repeat set to the current password length guessed.

Can start at 1 character passwords (or whatever your lower bound is) then cap it at a maximum length too. 

Then just return when match is found.

> Sample Output

a 1

b 2

c 3

d 4

...

aba 1369

abb 1370

password is abc. found in 1371 guesses.
