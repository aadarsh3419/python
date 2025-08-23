class Solution(object):
    def twoSum(self, nums, target):
        for i in range(len(nums)):
            for j in range(i + 1, len(nums)):
                if nums[i] + nums[j] == target:
                    return [i, j]

# Example usage
sol = Solution()
print(sol.twoSum([2, 7, 11, 15], 9))  # [0, 1]
print(sol.twoSum([3, 2, 4], 6))       # [1, 2]
print(sol.twoSum([3, 3], 6))          # [0, 1]
