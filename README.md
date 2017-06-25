# k-inverse-pairs

Given two integers n and k, find how many different arrays consist of numbers from 1 to n such that there are exactly k inverse pairs.

An inverse pair is defined as following: For ith and jth element in the array, if i < j and a[i] > a[j] then it's an inverse pair; Otherwise, it's not.

The answer should be modulo 10^9 + 7.

---------------------------------------------------------------------------------------------------------
My Solution is using the backtracking approach :
1. For a given 'n', It generates all possible permutations, passing each one by one to a MergeSort (inverse pair counting function)
2. If the number returned in equal to given 'k', then final ans is incremented (stored at the 0th index of an Integer List)

NOTE : This is a Leetcode question and this solution will not work for n>=10, however works correctly for lower values of n.
Time complexity :O(Nlog N * 2^N)
