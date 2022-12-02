# running-sum
..
class Solution {
public:
    vector<int> runningSum(vector<int>& nums) {
        int n= nums.size();
        vector<int> rsum(n);
        for(int i=0;i<n;i++){
            rsum[i]=0;
            for(int j=0;j<=i;j++){
                rsum[i]+=nums[j];
            }
        }
        return rsum;

        
    }
};
