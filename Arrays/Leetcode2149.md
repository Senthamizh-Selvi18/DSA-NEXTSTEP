class Solution {
    public int[] rearrangeArray(int[] nums) {
        int[] res= new int[nums.length];

        int posi = 0;
        int nega = 1; 

        for (int i = 0; i < nums.length; i++) {
            if (nums[i]> 0)
            {
                res[posi] = nums[i];
                posi+= 2;
            } 
            else
            {
                res[nega] = nums[i];
                nega+= 2;
            }
        }
        return res;
    }
}