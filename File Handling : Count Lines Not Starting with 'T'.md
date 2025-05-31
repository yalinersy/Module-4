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
def count_lines_not_starting_with_T():
    try:
        with open("story.txt", "r") as file:
            count = 0 
            for line in file:
                stripped_line = line.lstrip()
                if stripped_line and stripped_line[0] != 'T':
                    count += 1
        print(f"Number of lines not starting with 'T': {count}")

    except FileNotFoundError:
        print("The file 'story.txt' was not found.")
count_lines_not_starting_with_T()

```

## Output
![image](https://github.com/user-attachments/assets/1ed2457e-a7af-4d1e-ad3d-48b74d5fd0cb)


## Result
Thus,the program has been executed successfully.
