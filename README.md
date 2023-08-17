# Median-of-two-arrays
class Solution:
    def findMedianSortedArrays(self, nums1: List[int], nums2: List[int]) -> float:
        num=sorted(concat(nums1,nums2))
        a=len(num)//2
        if len(num)%2==0:
            b=(num[a]+num[a-1])/2
            return float(b)
        else:
            return float(num[a])
