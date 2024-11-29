Sorting Activities by Finish Time:

We sort the array 
𝑎
[
1..
𝑁
]
a[1..N] by their finish times using a standard sorting method like Merge Sort or Quick Sort.
Time Complexity: 
𝑂
(
𝑁
log
⁡
𝑁
)
O(NlogN).
Initialization:

The set 
𝐴
A is initialized with the first activity, and a variable prev is set to 1 to track the most recently added activity.
Time Complexity: 
𝑂
(
1
)
O(1).
Iterating Through Activities:

A loop runs from 
𝑖
=
2
i=2 to 
𝑁
N. For each activity, we check if its start time is greater than or equal to the finish time of the last selected activity (
𝑎
[
𝑝
𝑟
𝑒
𝑣
]
.
𝑓
𝑖
𝑛
𝑖
𝑠
ℎ
a[prev].finish).
If the condition is true, the activity is added to 
𝐴
A, and prev is updated.
Time Complexity of Loop: 
𝑂
(
𝑁
)
O(N).
Adding Activities (Union Operation):

Adding an activity to the set 
𝐴
A is done in constant time.
Time Complexity: 
𝑂
(
1
)
O(1).
Overall Time Complexity:
The sorting step, which takes 
𝑂
(
𝑁
log
⁡
𝑁
)
O(NlogN), dominates the total time.
The loop and adding activities take 
𝑂
(
𝑁
)
O(N).
So, the total time complexity is:
𝑂
(
𝑁
log
⁡
𝑁
)
+
𝑂
(
𝑁
)
=
𝑂
(
𝑁
log
⁡
𝑁
)
O(NlogN)+O(N)=O(NlogN)
