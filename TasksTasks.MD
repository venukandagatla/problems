Write a function:
public boolean solution(int numTasks, int[][] prerequisites)
that, given an integer numTasks and a zero-indexed array of array prerequisites consisting of numTasks paired integers, returns a boolean that if all the tasks can be completed.

Here is the complete problem statement with examples:

There is a total of numTasks tasks you must complete, labeled from 0 to (numTasks - 1). You are given an array prerequisites where prerequisites[i] = [ai, bi] indicates that you must complete the task bi first, if you want to complete the task ai.
•	For example, the pair [0, 1], indicates that to complete the task 0 you have to first complete the task 1.
Return true if you can complete all the tasks. Otherwise, return false.

Example 1:
Input: numTasks = 2, prerequisites = [[1,0]]
Output: true
Explanation: There are a total of 2 tasks to complete. 
To complete the task 1 you should have completed the task 0. So, it is possible.
Example 2:
Input: numTasks = 2, prerequisites = [[1,0],[0,1]]
Output: false
Explanation: There are a total of 2 tasks to complete. 
To complete the task 1 you should have completed task 0, and to complete task 0 you should also have completed the task 1. So it is impossible.
 
Constraints:
•	1 <= numTasks <= 2000
•	0 <= prerequisites.length <= 5000
•	prerequisites[i].length == 2
•	0 <= ai, bi < numTasks 
•	All the pairs prerequisites[i] are unique.
