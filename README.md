# python-project
pick random number for properties
#Python Program to Print Properties of user input number.

import random

a = int(input('Enter lower limit: '))
b = int(input('Enter upper limit: '))
c = random.randint(a,b)

print("\t \t \t User Choose The Number",str(c)+" !!\n")
print("\t \t \t Properties of Chosen Number  \n")

if c == 0:
    print("0 is neither negative nor positive ! \n")
else:     
    if c > 0:
        print(c,"is a positive number.\n")
    else:
        print(c,"is a negative number.\n")    
    if c % 2 == 0:
        print(c,"is an even number.\n")
    else:
        print(c,"is an odd number.\n")
    if c > 1:
        for j in range(2,c+1):
            if c % j == 0:
                print(c,'is a composite number.\n')
                break
            else:
                print(c,'is a prime number.\n')
                break
    elif c == 1:
        print("1 is neither Composite nor Prime ! \n")
    else:
        print('Negative numbers are neither Composite nor prime ! \n')

    
    
