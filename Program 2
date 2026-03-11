class Solution:
    def maxSubarraySum(self, arr):
        # Initialize with the first element
        # This handles arrays with all negative numbers correctly
        max_so_far = arr[0]
        current_max = arr[0]
        
        # Iterate from the second element onwards
        for i in range(1, len(arr)):
            # Decide: extend the previous subarray or start a new one?
            current_max = max(arr[i], current_max + arr[i])
            
            # Update the global maximum if the current subarray is better
            max_so_far = max(max_so_far, current_max)
            
        return max_so_far
        
