class Solution {
    public int missingNumber(int[] nums) {
        int no= 0;
        int n = nums.length;

        for (int i = 0; i <= n; i++) {
            no^= i;
        }

        for (int i = 0; i < n; i++) {
            no^= nums[i];
        }

        return no;
    }
}