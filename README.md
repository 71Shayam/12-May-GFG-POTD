 int minSteps(int d) {
        // code here
         int temp=0,ans=0;
        while(temp<d){
            ans++;
            temp+=ans;
        }
        if(temp==d)return ans;
        int diff=temp-d;
        if(diff%2==0)return ans;
        return ans%2==0?ans+1:ans+2;
    }
