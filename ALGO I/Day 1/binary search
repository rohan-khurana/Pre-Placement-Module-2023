class Solution:
    def search(self, nums: List[int], target: int) -> int:
        start = 0
        end = len(nums)

        # Binary Search
        while start < end:
            mid = ((end-start) // 2) + start
            # Mid point is target
            if nums[mid] == target:
                return mid
            # Mid point bigger than target
            elif nums[mid] > target:
                end = mid
            # Mid point smaller than target
            elif nums[mid] < target:
                start = mid+1

        return -1
