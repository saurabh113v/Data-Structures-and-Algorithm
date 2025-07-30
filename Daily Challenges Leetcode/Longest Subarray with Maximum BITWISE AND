class Solution {
    public int longestSubarray(int[] nums) {
        int maxNum = 0; // variable to store the maximum value in the array
        // Iterate through the array to find the maximum value
        for (int num : nums) {
            maxNum = Math.max(maxNum, num);
        }

        int maxLength = 0; // variable to store the length of the longest subarray
        int currentLength = 0; // variable to track the length of the current subarray

        // Iterate through the array to find the length of the longest subarray
        // where all elements are equal to the maximum value
        for (int num : nums) {
            if (num == maxNum) {
                // If the current element is the max, increment the current length
                currentLength++;
                // Update the maxLength if the current subarray is longer
                maxLength = Math.max(maxLength, currentLength);
            } else {
                // Reset the current length if the current element is not max
                currentLength = 0;
            }
        }
      
        // Return the length of the longest subarray
        return maxLength;
    }
}
