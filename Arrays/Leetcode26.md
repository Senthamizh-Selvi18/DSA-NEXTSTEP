class Solution {
    public int removeDuplicates(int[] nums) {
        int k=0;
        for (int i=0;i < numslength; i++) {
            if(i == 0 || nums[i]=nums[i - 1]) {
                nums[k]= nums[i];
                k++;
            }
        }
        return k;
    }
}