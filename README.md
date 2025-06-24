## 🔐 Random String Generator

*This simple Python script creates a text file filled with 100 random strings.*

*Each string is made up of letters, digits, and punctuation, and has a random length between 5 and 20 characters.*

### 📋 **What It Does**

- Generates 100 strings.

  
- Each string is made from a mix of:
  - Uppercase letters `A–Z`
  - Lowercase letters `a–z`
  - Numbers `0–9`
  - Special characters like `!@#$%^&*`
 
  
- Saves the strings in a file called `so Random strings.txt`, with one string per line.

### 🔍 How It Works

1. **Imports Required Modules**
2. ```
   import random
   import string
   ```

3. **Defines the `number(length)` Function**  
   It returns a random string of the given `length` by randomly choosing characters from letters, digits, and punctuation.

4. **Generates Random Strings**
   ```python
   for i in range(100):
       strings.append(number(random.randint(5, 20)))
   ```
   This loop creates 100 strings. Each string is randomly between 5 and 20 characters long.

5. **Prints the Strings with Line Numbers**
   ```python
   for i, s in enumerate(strings):
       print(i, '-', s)
   ```

6. **Writes the Strings to a File**
   ```python
   with open('so Random strings.txt','w') as done:
       for write in strings:
           done.write(write+'\n')
   ```

### 💡 Use Cases

- Dummy data for testing input fields
- Generating passwords (note: add extra security logic if used seriously)
- Text file stress tests

---
