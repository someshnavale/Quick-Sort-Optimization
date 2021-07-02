# Quick-Sort-Optimization

partition(A, low, high) is
pivot := A[high]
i := low
for j := low to high – 1 do
 if A[j] ≤ pivot then
 swap A[i] with A[j]
 i := i + 1
swap A[i] with A[high]
return i
Quick Sort mechanism :
quicksort(A, low, high) is
if low < high then
 p := partition(A, low, high)
 quicksort(A, low, p – 1)
 quicksort(A, p + 1, high)
 
 quicksort(A, lo, hi) is
if lo < hi then
 p := partition(A, lo, hi)
 quicksort(A, lo, p)
 quicksort(A, p + 1, hi)
Partition :
partition(A, lo, hi) is
pivot := A[lo]
i := lo - 1
j := hi + 1
loop forever
 do:
 i := i + 1
 
 while A[i] < pivot do

 do:
 j := j - 1
 while A[j] > pivot do

 if i >= j then
 return j

 swap A[i] with A[j]
