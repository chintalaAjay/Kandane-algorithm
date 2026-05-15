Kadane’s Algorithm | Maximum Subarray Sum

This project contains a Java solution for finding the Maximum Sum Subarray using Kadane’s Algorithm.

🚀 Problem Statement

Given an integer array arr[], find the contiguous subarray with the maximum sum and return that sum.

🔗 Problem Link:
GeeksforGeeks - Kadane’s Algorithm

💡 Approach Used

This solution uses Kadane’s Algorithm, an optimized approach for solving the Maximum Subarray Sum problem in linear time.

Main Idea
Traverse the array once.
Keep adding elements to the current sum.
If the current sum becomes negative, reset it to 0.
Continuously track the maximum sum obtained.
✅ Java Solution
class Solution {
    int maxSubarraySum(int[] arr) {

        int sum = 0;
        int max = Integer.MIN_VALUE;

        for(int i = 0; i < arr.length; i++) {

            sum += arr[i];

            if(sum > max) {
                max = sum;
            }

            if(sum < 0) {
                sum = 0;
            }
        }

        return max;
    }
}
📊 Time Complexity

O(n)

Only one traversal of the array is required.

📦 Space Complexity

O(1)

No extra space is used except variables.

🔥 What I Learned
Understanding Kadane’s Algorithm
Optimizing from brute force approach
Importance of resetting negative sums
Improving problem-solving and debugging skills
🛠️ Tech Stack
Java
DSA
Arrays

⭐ Practicing DSA consistently to improve problem-solving skills and prepare for coding interviews.
