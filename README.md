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
