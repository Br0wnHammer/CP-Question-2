# CP-Question-2
Again Stuck at a medium Level questions.

Manasa is out on a hike with friends. She finds a trail of stones with numbers on them. She starts following the trail and notices that any two consecutive stones' numbers differ by one of two values. Legend has it that there is a treasure trove at the end of the trail. If Manasa can guess the value of the last stone, the treasure will be hers.

For example, assume she finds 2 stones and their differences are a=2 or b=3. We know she starts with a 0 stone not included in her count. The permutations of differences for the two stones would be [2,2],[2,5],[3,5[,[3,6] or . Looking at each scenario, [2,2],[2,5],[3,2],[3,3] stones might have  or  on them. The last stone might have any of , or  on its face.

Compute all possible numbers that might occur on the last stone given a starting stone with a  on it, a number of additional stones found, and the possible differences between consecutive stones. Order the list ascending.

# Function Description

Complete the stones function in the editor below. It should return an array of integers representing all possible values of the last stone, sorted ascending.

stones has the following parameter(s):

n: an integer, the number of non-zero stones
a: one possible integer difference
b: another possible integer difference

# Input Format

The first line contains an integer , the number of test cases.

Each test case contains  lines:
- The first line contains , the number of non-zero stones found.
- The second line contains , one possible difference
- The third line contains , the other possible difference.

# Sample Input

2
3 
1
2
4
10
100

# Sample Output

2 3 4 
30 120 210 300 

# Explanation

With differences 1 and 2, all possible series for the first test case are given below:

0,1,2
0,1,3
0,2,3
0,2,4
Hence the answer 2 3 4.

With differences 10 and 100, all possible series for the second test case are the following:

0, 10, 20, 30
0, 10, 20, 120
0, 10, 110, 120
0, 10, 110, 210
0, 100, 110, 120
0, 100, 110, 210
0, 100, 200, 210
0, 100, 200, 300
Hence the answer 30 120 210 300.
