class Solution {
    public List<Integer> majorityElement(int[] nums) {
        int n=nums.length;
        int max=n / 3;
        List<Integer> result= new ArrayList<>();
     for (int i=0;i<n;i++) {
            int count=0;
        for (int j=0;j<n;j++) {
                if(nums[i]== nums[j]) count++;
            }
        if (count>max && !result.contains(nums[i])) result.add(nums[i]);
        }
        return result;
    }
}