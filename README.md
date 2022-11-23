# Baseconverter
Converts numbers from one base to another (supports negative bases)

How to convert to negative bases?

Converting a number to base 10 given the base is really easy. All you do is take each digit starting from the right, then multiply said digit by the base to the power of how many spaces from the right it is, then add

For example, with the number 234 to base 5, you would do (4*5^0) + (3*5^1) + (2*5^2) --> 4*1 + 3*5 + 2*25 --> 4 + 15 + 50 --> 69

This method works with any base, positive,negative, or imaginary, which is likely going to be my next project


To convert from base 10 to a specified base, you would use the remander to find the digits starting from the right

For example: 70 to base -3
70 is not divisble by 3,but 70-((-3^0)*1), or 69 is, so the first digit is 1
69 is not divisble by 9, but 69 - ((-3^1)*1), or 72 is, so the next digit is 1
72 is not divisble by 27, but 72 - ((-3^2)*2), or 54 is, so the next digit is 2
54 is not divisble by 81, but 54 - ((-3^3)*1), or 81 is, so the next digit is 1
81 is not divisble by 243, but 81 - ((-3^4)*1), or 0 is, so the next digit is 1

Since we've reached zero, all of our digits combined must equal 70, so 70 in base -3 equals 11211
If we use the method from before, we get (1*81 - 1*27 + 2*9 - 1*3 + 1), which equals 70
