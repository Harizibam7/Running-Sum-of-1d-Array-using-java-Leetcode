# Running-Sum-of-1d-Array-using-java-Leetcode
    class Solution {
        public int[] runningSum(int[] nums) {
            int n = nums.length;
            int arr[] = new int[n];
    
            for(int i = 0;i<n;i++){
                int sum =0;
                for(int j =0;j<i+1;j++){
                        sum = sum + nums[j];
                }
                arr[i] = sum;
            }
            return arr;
        }
    }
