# Problems
merge sorted array
You are given two integer arrays nums1 and nums2, sorted in non-decreasing order, and two integers m and n, representing the number of elements in nums1 and nums2 respectively.

Merge nums1 and nums2 into a single array sorted in non-decreasing order.
class Solution:
    def merge(self, nums1: List[int], m: int, nums2: List[int], n: int) -> None:
        for i in range(n):
            nums1.remove(0)
            nums1.append(nums2[i])
        nums1.sort() 
