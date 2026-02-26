class Solution {
    public int maxProfit(int[] prices) {
        int max=0;
        int diff=0;
       for(int i=0;i<prices.length;i++){
        for(int j=1;j<prices.length;j++){
        if(prices[i]<prices[j]){
            diff=prices[j]-prices[i];
        }
        if(diff>max){
            max=diff;
        }
       } 
       }
   return max;
    }
}