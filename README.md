# 3nplus1
Computacional representation of th 3x + 1 problem.

import matplotlib.pyplot as plt

x = eval(input('Write any number you like: ')) #Choose any number you think may refutate this theorem#
a = [x]
while x > 1:
    if x % 2 == 0:
        x = x/2
    else:
        x = (3 * x) + 1
    y = a.append(x)
    print(x)

b = []

for i in range(len(a)):
    b.append(i + 1)

print('Number of steps: ', len(a))
plt.plot(b, a)
plt.grid(True)
plt.show()
