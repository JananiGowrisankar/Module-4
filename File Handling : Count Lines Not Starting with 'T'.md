# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
```
count = 0
try:
    with open('story.txt', 'r') as file:
        for line in file:
            line = line.strip() 
            if line and not line.startswith('T'):
                count += 1
    print("Number of lines not starting with 'T':", count)

except FileNotFoundError:
    print("File not Found")

```
## Output

![image](https://github.com/user-attachments/assets/cdb590a9-627c-49cc-9439-22e01d608be0)


## Result
Thus a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'` is successfully verified.
