# Exp.No:18  
## FILES - FREQUENCY OF CHARACTERS IN A FILE

### AIM  
To write a Python program that reads a file and counts the frequency of each character in it.

### ALGORITHM

1. Begin the program.
    
2. Define the function `create_file()` that accepts two arguments:  
   - `file_path`: The path to the file.  
   - `content`: The string content to be written into the file.
       
3. Open the file specified by `file_path` in write mode (`'w'`), and write the provided `content` into the file.
   
4. Close the file (this is automatically done when exiting the `with` block).
   
5. Define the function `character_frequency()` that accepts one argument:  
   - `file_path`: The path to the file whose character frequency is to be calculated.
       
6. Open the file specified by `file_path` in read mode (`'r'`), and read its content into the variable `content`.
    
7. Initialize an empty dictionary (`d1`) to store the frequency of each character using `defaultdict(int)`.
  
8. Loop through each character in the `content`:  
   - For each character `ch`, increment its corresponding frequency in the dictionary `d1`.
      
9. Return the dictionary `d1`, which contains the frequency of each character in the file.
     
10. Terminate the program.


### PROGRAM

```
# Reg.No-212223020020
# Name-Pradaksha V
from collections import defaultdict

def create_file(file_path, content):
    """Creates a file with the given content."""
    with open(file_path, 'w') as file:
        file.write(content)

def character_frequency(file_path):
    """Returns the frequency of each character in the specified file."""
    with open(file_path, 'r') as file:
        content = file.read()
    
    d1 = defaultdict(int)
    for ch in content:
        d1[ch] += 1
    
    return dict(d1)  # Convert defaultdict back to a regular dict for clarity

# Example usage
#Corrected the variable name from 'name' to '_name_'
if _name_ == "_main_":  
    # Create a sample file
    file_path = "sample.txt"
    sample_content = "hello world!"
    create_file(file_path, sample_content)
    
    # Calculate character frequencies
    freq = character_frequency(file_path)
    
    # Print the frequencies
    print("Character frequencies in the file:")
    for char, count in freq.items():
        print(f"'{char}': {count}")

```
### OUTPUT
![WhatsApp Image 2025-04-28 at 23 26 28_759baa41](https://github.com/user-attachments/assets/bca63a1c-6824-4d3d-8e69-df8a5ad7f7d4)


### RESULT
The program counts the frequency of each character in a file by reading its content, then using a dictionary to track how many times each character appears, with the final output displaying each character and its corresponding count.
