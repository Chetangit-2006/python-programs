#  Basic python-programs
//Access and print characters from the string
s = "Python"
print(s[0])     # First character
print(s[-1])    # Last character


//Print a string and extract characters
s = "Hello"
print("String is:", s)
for ch in s:
    print(ch)

    
// Print words with their length
s = "Python is easy"
words = s.split()
for w in words:
    print(w, "=", len(w))

    
// Print EVEN length words
s = "Python is very easy"
words = s.split()
for w in words:
    if len(w) % 2 == 0:
        print(w)

        
// Count vowels in a string
s = "Hello World"
vowels = "aeiouAEIOU"
count = 0
for ch in s:
    if ch in vowels:
        count += 1
print("Vowels:", count)


// Passing string value to function
def greet(name):
    print("Hello", name)
greet("Aryan")


// Multiple copies using *
s = "Hi "
print(s * 3)


// Append text using +=
s = "Hello"
s += " World"
print(s)


//Concatenate using +
s1 = "Hello"
s2 = "Python"
s3 = s1 + " " + s2
print(s3)


//Check substring using in
s = "Python Programming"
if "Python" in s:
    print("Substring found")

    
// Assign Hexadecimal values
s = "\x48\x65\x6C\x6C\x6F"
print(s)


//Print double quotes
s = "He said, \"Hello\""
print(s)


//Ignore escape sequences (raw string)
s = r"Hello\nWorld"
print(s)


//Count all possible substrings
s = "abc"
n = len(s)
count = n * (n + 1) // 2
print("Total substrings:", count)


//Reverse string (5 ways)
s = "Python"
# 1. Slicing
print(s[::-1])
# 2. Loop
rev = ""
for ch in s:
    rev = ch + rev
print(rev)
# 3. reversed() function
print("".join(reversed(s)))
# 4. While loop
i = len(s)-1
while i >= 0:
    print(s[i], end="")
    i -= 1
# 5. Recursion
def reverse_str(st):
    if len(st) == 0:
        return st
    return reverse_str(st[1:]) + st[0]
print("\n", reverse_str(s))


// Reverse using stack & reversed()
# Using stack
s = "Python"
stack = list(s)
rev = ""
while stack:
    rev += stack.pop()
print("Stack Reverse:", rev)
// Using reversed()
print("Reversed Method:", "".join(reversed(s)))


//Split string into characters
s = "Python"
arr = list(s)
print(arr)


//String slicing
s = "Python Programming"
print(s[0:6])
print(s[7:])
print(s[::-1])


// Repeat M characters N times
s = "Python"
m = 3
n = 2
print((s[:m]) * n)


#Swap characters in string
s = "abcd"
//Swap first and last
new_s = s[-1] + s[1:-1] + s[0]
print(new_s)
