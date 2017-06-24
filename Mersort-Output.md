## Original Output

```
C:\Users\sanan\CLionProjects\p1\cmake-build-debug\untitled.exe
Enter a number of elements to be inside the array to be sorted
7
Enter 7 numbers:
67
9
76
69
23
7
98

Originally entered array is:
67
9
76
69
23
7
98
The length of the array is:
7
Enter the choice you want to make a->Insertion Sort, b->insertionsort_noninc, c->MergeSort
c
Merge Sort :
Values: p1=0, q1=3, r1=6
Values: p1=0, q1=1, r1=3
Values: p1=0, q1=0, r1=1
Values: p1=2, q1=2, r1=3
Values: p1=4, q1=5, r1=6
Values: p1=4, q1=4, r1=5
7
9
23
67
69
76
98

Process finished with exit code 0
```
## Output Explained
```rust
-----------------------------------------------
output
A = [3, 41, 52, 26, 38, 57, 9, 49]

-- Output
Originally entered array is:
3  [0]
41 [1]
52 [2]
36 [3]
38 [4]
57 [5]
9  [6]
49 [7]

The length of the array is:
8

Merge Sort :

The Logic goes from bottom to top:

Values: p1=2, q1=2, r1=3

Size of the array=1
52
Size of the array=1
36
 -- loop - k=2
value of k , n1,  n2, 2, 1, 1
value of l , m, 0, 0
chk-3, 36
 -- loop - k=3 	
value of k , n1,  n2, 3, 1, 1
value of l , m, 0, 1
chk-4, array : 52, 36, 3
array at the end
Size of the array=2
3 41
Size of the array=2
3 41
Size of the array=2
36 52

[0] 3
[1] 41
[2] 36
[3] 52
--call at A[0,3], p=0, q=1, r=3 , n1=2, n2=2
value of k , n1,  n2, 0, 2, 2
value of l , m, 0, 0
chk-2, 3
value of k , n1,  n2, 1, 2, 2
value of l , m, 1, 0
chk-3, 36
value of k , n1,  n2, 2, 2, 2
value of l , m, 1, 1
chk-2, 41
value of k , n1,  n2, 3, 2, 2
value of l , m, 2, 1
chk-5, array : 52, 52, 3
array at the end
Size of the array=2
3 36

--call at A[4,7]
	[4,5] [6,7]
	[4] [5]
Values: p1=4, q1=5, r1=7
Values: p1=4, q1=4, r1=5
Size of the array=1
38
Size of the array=1
57
value of k , n1,  n2, 4, 1, 1
value of l , m, 0, 0
chk-2, 38
value of k , n1,  n2, 5, 1, 1
value of l , m, 1, 0
chk-5, array : 57, 57, 5
array at the end
Size of the array=2
3 36

-- call at [6,7]
Values: p1=6, q1=6, r1=7
Size of the array=1
9
Size of the array=1
49
value of k , n1,  n2, 6, 1, 1
value of l , m, 0, 0
chk-2, 9
value of k , n1,  n2, 7, 1, 1
value of l , m, 1, 0
chk-5, array : 49, 49, 7
array at the end
Size of the array=2
3 36
Size of the array=2
38 57
Size of the array=2
9 49

-- call for A[4,7], p=4,q=5,r=7, n1=2,n2=2
value of k , n1,  n2, 4, 2, 2
value of l , m, 0, 0
chk-3, 9
value of k , n1,  n2, 5, 2, 2
value of l , m, 0, 1
chk-2, 38
value of k , n1,  n2, 6, 2, 2
value of l , m, 1, 1
chk-3, 49
value of k , n1,  n2, 7, 2, 2
value of l , m, 1, 2
chk-4, array : 57, 49, 7
array at the end
Size of the array=2
3 36
Size of the array=4
3 36 41 52
Size of the array=4
9 38 49 57

-- call for A[0,7] ,p=0, q=3, r=7, n1=4, n2=4
value of k , n1,  n2, 0, 4, 4
value of l , m, 0, 0
chk-2, 3
value of k , n1,  n2, 1, 4, 4
value of l , m, 1, 0
chk-3, 9
value of k , n1,  n2, 2, 4, 4
value of l , m, 1, 1
chk-2, 36
value of k , n1,  n2, 3, 4, 4
value of l , m, 2, 1
chk-3, 38
value of k , n1,  n2, 4, 4, 4
value of l , m, 2, 2
chk-2, 41
value of k , n1,  n2, 5, 4, 4
value of l , m, 3, 2
chk-3, 49
value of k , n1,  n2, 6, 4, 4
value of l , m, 3, 3
chk-2, 52
value of k , n1,  n2, 7, 4, 4
value of l , m, 4, 3
chk-5, array : 57, 57, 7
array at the end
Size of the array=2
3 9
3
9
36
38
41
49
52
57
```
