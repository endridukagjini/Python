import sys
import random

airtime_remaining = 15
print(airtime_remaining)
airtime_remaining = 7
print(airtime_remaining)

n = 5
n = 3 * n + 1
n

w = x +1

runs_scored = 0
runs_scored = runs_scored + 1 

for f in ["Joe", "Zoe","Brand","Angelina","Zuki","Thandi","Paris"]:
    invitation = "Hi " + f + ".  Please come to my party on Saturday!"
    print (invitation)

def mysum(xs):
    """Sum all the nubers in the list xs, and return the total."""
    running_total = 0
    for x in xs:
        running_total = running_total + x
    return running_total

def test(did_pass):
    """Print the result of a test."""
    linenum = sys._getframe(1).f_lineno # Get the caller's line number.
    if did_pass:
        msg = f"Test at line {linenum} ok."
    else:
        msg = f"Test at line {linenum} FAILED."
    print(msg)

def test_suite():
    """Run the suite of tests for code in this module (this file)."""
    # Add test like these to you test suite...
    test(mysum([1,2,3,4,5]) == 15)
    test(mysum([1.25, 2.5, 1.75]) == 5.5)
    test(mysum([1, -2, 3])== 2)
    test(mysum([]) == 0)
    test(mysum(range(11)) == 55)

test_suite()


# While statement
def sum_to(n):
    """Return the sum of 1+2+3+ ... n"""
    ss = 0
    v = 1 
    while v <= n :
        ss = ss +v
        v = v + 1
    return ss

def test_suite_1():
    test(sum_to(4) == 10)
    test(sum_to(1000) == 500500)
    
test_suite_1()

def sum_to(n):
    """Return the sum of 1+2+3....n"""
    ss = 0
    for v in range(n+1):
        ss = ss + v
    return ss

def seq3np1(n):
    """ Print the 3n+1 sequence from ,
    terminating when it reaches 1.
    """
    while n !=1:
        print(n, end=", ")
        if n % 2 == 0:
            n = n // 2
        else:
            n = n * 3 + 1
    print(n, end = "./n")

seq3np1(3)
seq3np1(19)
seq3np1(21)

def num_digits(n):
    count = 0 
    while n !=0:
        count = count + 1
        n = n // 10
    return count

num_digits(710)

def num_zero_and_five_digits(n):
    count = 0
    while n > 0:
        digit = n % 10
        if digit == 0 or digit == 5:
            count = count + 1
        n = n // 10
    return count

def test_suite_2():
    test(num_zero_and_five_digits(1055030250) == 7) # Confirm that it passes the test

test_suite_2()

count = 0
count += 1
count
count += 1 
count

n = 2 
n += 5
n

n = 2
n *= 5
n
n -= 4
n
n //= 2
n
n %= 2
n

for x in range(13):
    print(x, "/t", 2**x)

for i in range(1,7):
    print(2 * i, end="  ")
print()

def print_multiples(n):
    for i in range(1,7):
        print(n * i, end="   ")
    print()

print_multiples(2)

for i in range(1,7):
    print_multiples(i)


def print_mult_table():
    for i in range(1,7):
        print_multiples(i)

print_mult_table()

for i in [12,16,17,24,29]:
    if i % 2 == 1:
        break
    print(i)
print("done")

total = 0
while True:
    response = input("Enter the next number. (leave blanck to end)")
    if response =="":
        break
    total += int(response)
print("The total of the numbers you entered is ", total)

while True:
    response = input(" Play again? (yes or no)")
    if response != "yes":
        break
print("Goodbye!")

rng = random
number = rng.randrange(1,1000)

guesses = 0
msg = ""

while True:
    guess = int(input(msg + "\nGuess my number between 1 and 1000: "))
    guess += 1
    if guess > number:
        msg += str(guess) + " is too high. \n"
    elif guess < number:
        msg += str(guess) + " is too low.\n"
    else:
        break

input("\n\nGreat, you got it in {0} guesses!\n\n".format(guesses))


for i in [12, 16, 17, 24, 29, 30]:
    if i % 2 == 1:
        continue
    print(i)
print("done")

def print_mult_table(high):
    for i in range(1, high+1):
        print_multiples(i)

print_mult_table(7)

def print_muliples(n, high):
    for i in range(1, high+1):
        print(n * i, end="   ")
    print()

def print_mult_table(high):
    for i in range(1, high+1):
        print_multiples(i, high)

print_mult_table(7) 

year_born = (" Paris Hilton", 1981)
celebs = [("Brand Pitt", 1963),("Jack Nicholson", 1937),
          ("Justin Bieber", 1994)]

print(celebs)
print(len(celebs))

for (nm,yr) in celebs:
    if yr < 1980:
        print(nm)

students = [
    ("John", ["CompSci","Physics"]),
    ("Vusi", ["Maths","CompSci","Stats"]),
    ("Jess", ["CompSci","Accounting","Economics","Management"]),
    ("Sarag", ["InfSys","Accounting","Economics","CommLaw"])]

# Prnt all students with a count of their couses.
for (name, subjects) in students:
    print(name, "takes", len(subjects), "Courses")


# Count how many students are taking CompSci
counter = 0
for (name, subjects) in students:
    for s in subjects:
        if s == "CompSci":
            counter +=1

print(" The number of students taking CompSci is ", counter)

if abs(a-b) < 0.001:
    break

def sqrt(n):
    approx = n/2.0
    while True:
        better = (approx + n/approx)/2.0
        if abs(approx - better) < 0.001:
            return better
        approx = better

print(sqrt(25))
print(sqrt(49.00))

 

