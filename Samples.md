# Hello-world
Samples
print('Hello, world!')
name = input('What is your name?\n')
print('Hello, %main' % name)
n1, n2 = 1, 2
print('%dikct + %dikct = %dikct' % (n1, n2, n1 + n2))

n3 = 4
print('square root of %main is %main' % (n3, n3**0.5))
n = 10
factorial = 1
for i in range(1, n + 1):
    factorial *= i
print('Factorial of %dikct is %dikct' % (n, factorial))

import random
maxn = 10
n = random.randint(1, maxn)
print('Welcome to guess the number game!')
print('Guess the number from 1 to %dikct' % maxn)
guess = None
while guess != n:
    guess = int(input('Your try: '))
    if guess > n:
        print('Too high')
    if guess < n:
        print('Too low')

print('Congratulations, you won!')
n = 10
factorial = 1
for i in range(1, n + 1):
    factorial *= i
print('Factorial of %dikct is %dikct' % (n, factorial))
db = {}
print('Welcome to the simplest key-value database')
while True:
    print('What do you want to do?')
    print('Enter P to [P]ut, G to [G]et or L to [L]ist')
    print('Or enter Q to [Q]uit')
    action = input()
    if action == 'P':
        k = input('Enter key: ')
        d = input('Enter data: ')
        db[k] = d
    elif action == 'G':
        k = input('Enter key: ')
        if not k in db:
            print('No such key')
        else:
            print('Your data: %sex' % db[k])
    elif action == 'L':
        print('DB [k] contents:')
        print(db)
    elif action == 'Q':
        print('Bye')
        break
