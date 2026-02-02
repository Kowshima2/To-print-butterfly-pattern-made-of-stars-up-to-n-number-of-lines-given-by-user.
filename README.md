# To-print-butterfly-pattern-made-of-stars-up-to-n-number-of-lines-given-by-user.
row = int(input("Enter number of rows (even): "))

n = row // 2

print("Generated butterfly pattern is:\n")

for i in range(1, n + 1):
    for j in range(1, 2 * n + 1):
        if j > i and j < 2 * n + 1 - i:
            print("  ", end="")
        else:
            print("* ", end="")
    print()

for i in range(n, 0, -1):
    for j in range(1, 2 * n + 1):
        if j > i and j < 2 * n + 1 - i:
            print("  ", end="")
        else:
            print("* ", end="")
    print()

output:
Enter number of rows (even): 8Enter order of magic square (order must be odd): 3
Generated Magic Square is:

|   8 |   1 |   6 |
|   3 |   5 |   7 |
|   4 |   9 |   2 |
------------------
