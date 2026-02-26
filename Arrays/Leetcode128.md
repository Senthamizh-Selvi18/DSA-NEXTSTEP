import java.util.*;
class Solution {
    public int longestConsecutive(int[] nums) {
        Arrays.sort(nums);
        int count = 1;
        int Long=1;  
        if(nums.length==0){
                return 0;
        }
for (int i =1; i < nums.length; i++) {
            if (nums[i] == nums[i - 1] + 1)
            {
                 count++;
            }
            else if (nums[i] != nums[i - 1]) {
                count = 1;
            }
             if(count>Long){
                Long=count;
            }
        }

        return Long;
    }
}