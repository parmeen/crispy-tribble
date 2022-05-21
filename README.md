# crispy-tribble
'''
wipro-previous-years-questions
Write a program to find the transpose of a given n*m matrix.

Input Format:

First line take an Integer from stdin  which is number of rows n.
Second line take an Integer from stdin which is number of columns m.
Third line take an Integers which are matrix elements
Output Format:

Transpose of a matrix

Example Input:

1   2   3
4   5   6
7   8   9


Output:

1   4   7
2   5   8
3   6   9
''' 
import numpy
n=int(input())
m=int(input())
matrix=list(input().split())
mat=numpy.array_split(matrix,n)
trans=numpy.transpose(mat)
for i in trans:
    for j in i:
        print(j,end=" ")
    print("\n",end="")
