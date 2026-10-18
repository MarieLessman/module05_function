# debug_log.md
# Author: Marie Lessman

## Bug 1
Error type: KeyError
File + line: week8_buggy.py line 12 (called from line 21).
What the error means: Python looked for the key 'amount' in the first record but it wasn't there. In line 4 there was a typo in the spelling 'amout' which is supposed to be 'amount'. It was not able to find the certain key it was looking for and because of that line 12 and 21 was not able to function. 
What I told the duck: total starts at 0, then for each record it adds rec['amount']. Oh, the first record says 'amout'. So there's no 'amount' key to add.
What I tried: I put the debug print in and it showed me which record it crashed on.  
How I fixed it: I changed the typo in line 4 from 'amout' to 'amount'. 

## Bug 2
Error type: TypeError 
File + line: Week8_buggy.py line 16
What the error means: It was comparing a number to a string. Python can't use > between an int and '1000' becuse the quotes make it text (string) and not a number (integer).
How I fixed it: I changed the '1000' to 1000 since it is meant to be an integer and not a string.

## After Fixing Both Bugs
Final output: Total: $5150.00 across 3 records. True 
Did pytest pass? y/n: YES

## AI Literacy Reflection
Did I use AI? y/n: no
If yes -- exact prompt I used:
What AI explained:
What I changed myself:
Can I explain every fixed line? y/n: YES

## What I learned
I learned that a KeyError usually means a key name doesn't match, so a small typo can break the whole function. I also learned that a TypeError can come from quotes around a number. Reading the traceback from the bottom up showed me where to look first. 
