class Solution {
    public boolean check(int[] nums) {
        int order = 0;
        int len = nums.length;
for (int i = 0; i < len - 1; i++) {
  if (nums[i] > nums[i + 1]) {
                order++;
            }
        }

        if (nums[len - 1] > nums[0]) 
        {
            order++;
        }

        return order <= 1;
    }
}
