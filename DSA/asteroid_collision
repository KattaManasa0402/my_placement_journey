class Solution {
public:
    vector<int> asteroidCollision(vector<int>& a) {
        vector<int>st;
        int n=a.size();
        for(int i=0;i<n;i++){
            if(a[i]>0){
                st.push_back(a[i]);
            }
            else{
            while(!st.empty() && st.back()>0 && st.back()<abs(a[i])){
                st.pop_back();
            }
            if(!st.empty() && st.back()>0 && st.back()==abs(a[i])){
                st.pop_back();
            }
            else if(st.empty() || st.back()<0){
                st.push_back(a[i]);
            }
        }
        }
        return st;
    }
};
