# SET B QUESTION – 01

1. Prompt user to input a string and store it in the variable 'string'.
2. Initialize a variable 'vowels' to 0.
3. Define a string 'vowel' containing all vowel characters: "aeiouAEIOU".
4. Iterate through each character 'i' in the input string:
   a. Check if 'i' is present in the 'vowel' string.
   b. If yes, increment the 'vowels' count by 1.
5. Calculate the number of consonants by subtracting the number of vowels from the total length of the string.
6. Display the count of vowels and consonants using formatted strings.

Pseudocode:
Input: string
Output: Number of vowels, Number of consonants

string = input("Enter string:")
vowels = 0
vowel = "aeiouAEIOU"

for i in string:
    if i in vowel:
        vowels = vowels + 1

consonents = length(string) - vowels

print("Number of vowels are:", vowels)
print("Number of consonants are:", consonents)





# SET B QUESTION – 02

1. Function input_matrix(rows, cols):
   a. Initialize an empty list 'matrix'.
   b. Display a prompt to enter the elements for an `rows x cols` matrix.
   c. Iterate through each row 'i' in the range of 'rows':
      i. Initialize an empty list 'row'.
      ii. Iterate through each column 'j' in the range of 'cols':
          A. Prompt the user to enter an element at position (i+1, j+1) and store it in 'element'.
          B. Convert 'element' to a float and append it to the 'row' list.
      iii. Append the 'row' list to the 'matrix' list.
   d. Return the 'matrix'.

2. Function matrix_multiply(A, B):
   a. Get the number of rows and columns for matrices A and B.
   b. Check if the number of columns in A is equal to the number of rows in B; if not, return an error message.
   c. Initialize an empty matrix 'result' with dimensions (rows_A x cols_B) filled with zeros.
   d. Perform matrix multiplication using three nested loops:
      i. Iterate through each row 'i' in the range of rows_A:
         ii. Iterate through each column 'j' in the range of cols_B:
             A. Iterate through each element 'k' in the range of cols A:
                 a. Update the result[i][j] by adding the product of A[i][k] and B[k][j].
   e. Return the 'result' matrix

3. Function main():
   a. Prompt the user to enter the number of rows and columns for matrix A.
   b. Call input matrix function with rows A and cols A as arguments to get matrix A.
   c. Prompt the user to enter the number of rows and columns for matrix B.
   d. Call input matrix function with rows B and cols B as arguments to get matrix B.
   e. Call matrix multiply function with matrix A and matrix B as arguments to get the result.
   f. Display the result matrix.

4. Check if the script is being run as the main program:
   a. If true, call the main() function.

Pseudocode:
Function input_matrix(rows, cols):
   matrix = []
   Display prompt for matrix elements
   For each row i in range(rows):
      row = []
      For each column j in range(cols):
         element = Get input for element at position (i+1, j+1)
         Append float(element) to row
      Append row to matrix
   Return matrix

Function matrix_multiply(A, B):
   rows A, cols A = Get dimensions of A
   rows B, cols B = Get dimensions of B
   If cols A != rows B:
      Return "Error: Matrices cannot be multiplied; since the number of columns in A is not equal to the number of rows in B."
   result = Create matrix filled with zeros of dimensions (rows A x cols B)
   For each row i in range(rows A):
      For each column j in range(cols B):
         For each element k in range(cols A):
            result[i][j] += A[i][k] * B[k][j]
   Return result

Function main():
   rows A, cols A = Get input for rows and columns of matrix A
   matrix A = Call input matrix with rows A, cols A
   rows B, cols B = Get input for rows and columns of matrix B
   matrix B = Call input matrix with rows B, cols B
   result = Call matrix_multiply with matrix A, matrix B
   Display result

If script is being run as the main program:
   Call main()



# SET B QUESTION – 03

1. Create an empty list 'list1'.
2. Prompt the user to enter the size of the list and store it in the variable 'size'.
3. Display a message asking the user to enter values inside the list.
4. Iterate 'i' over the range from 0 to 'size - 1':
   a. Prompt the user to enter a value and store it in the variable 'values'.
   b. Convert 'values' to an integer and append it to 'list1'.
5. Display 'list1'.

6. Create an empty list 'list2'.
7. Prompt the user to enter the size of the second list and store it in the variable 'size2'.
8. Display a message asking the user to enter values inside the second list.
9. Iterate 'i' over the range from 0 to 'size2 - 1':
   a. Prompt the user to enter a value and store it in the variable 'values'.
   b. Convert 'values' to an integer and append it to 'list2'.
10. Display 'list2'.

11. Create an empty list 'similar_elements'.
12. Iterate over each element 'a' in 'list1':
   a. Iterate over each element 'b' in 'list2':
       i. If 'a' is equal to 'b', append 'a' to 'similar_elements'.

13. Display the list of similar elements.

Pseudocode:
1. list1 = []
2. size = Get input for the size of the list
3. Display message to enter values inside the list
4. For each element i in range(0, size):
   a. values = Get input for a value
   b. Append int(values) to list1
5. Display list1

6. list2 = []
7. size2 = Get input for the size of the second list
8. Display message to enter values inside the second list
9. For each element i in range(0, size2):
   a. values = Get input for a value
   b. Append int(values) to list2
10. Display list2
11. similar elements = []
12. For each element a in list1:
   a. For each element b in list2:
       i. If a equals b, append a to similar elements
13. Display similar elements


 # SET B QUESTION - 04

1. Input: rows, columns (number of rows and columns for matrix A)
2. Initialize an empty list A (matrix A)
3. Display a message: "Enter the elements for matrix A:"
4. For each row 'i' in the range from 0 to rows-1:
   a. Initialize an empty list 'a'
   b. For each column 'j' in the range from 0 to columns-1:
      i. Prompt the user to enter an element at position (i+1, j+1) and store it in 'values'
      ii. Convert 'values' to an integer and append it to 'a'
   c. Append 'a' to 'A'
5. Display the matrix A:
   a. For each row in A:
      i. Display the row

6. Initialize an empty list 'transpose A'
7. Calculate the transpose of matrix A:
   a. For each column 'i' in the range from 0 to columns-1:
      i. Initialize an empty list 'transposed row'
      ii. For each row 'j' in the range from 0 to rows-1:
          A. Append A[j][i] to 'transposed row'
      iii. Append 'transposed row' to 'transpose A'

8. Display the transpose of matrix A:
   a. For each row in transpose A:
      i. Display the row

Pseudocode:
1. rows = Get input for the number of rows
2. columns = Get input for the number of columns
3. A = Create an empty list for matrix A
4. Display "Enter the elements for matrix A:"
5. For each row i in range(0, rows):
   a. a = Create an empty list for the current row
   b. For each column j in range(0, columns):
      i. values = Get input for the element at position (i+1, j+1)
      ii. Append int(values) to a
   c. Append a to A
6. Display "Matrix A:"
7. For each row in A:
   a. Display the row

8. transpose A = Create an empty list for the transpose of matrix A
9. For each column i in range(0, columns):
   a. transposed row = Create an empty list for the current transposed row
   b. For each row j in range(0, rows):
      i. Append A[j][i] to transposed row
   c. Append transposed row to transpose A

10. Display "Transpose of Matrix A:"
11. For each row in transpose A:
    a. Display the row
