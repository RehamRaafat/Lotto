#include <bits/stdc++.h>

using namespace std;

int main()
{
    int K;
    bool onecase=false;
    while(cin>>K&&K)
    {
        if(onecase)
            cout<<endl;
        onecase=true;
        vector<int>v;
    for(int p=0; p<K; p++)
    {
        int x;
        cin>>x;
        v.push_back(x);
    }
    for(int i=0; i<v.size(); i++)
    {
        for(int j=i+1; j<v.size(); j++)
        {
            for(int k=j+1; k<v.size(); k++)
            {
                for(int l=k+1; l<v.size(); l++)
                {
                    for(int m=l+1; m<v.size(); m++)
                    {
                        for(int n=m+1; n<v.size(); n++)
                        {
                            if(v[i]!=v[j]!=v[k]!=v[l]!=v[m]!=v[n])
                            cout<<v[i]<<" "<<v[j]<<" "<<v[k]<<" "<<v[l]<<" "<<v[m]<<" "<<v[n]<<endl;
                            else
                                continue;
                        }
                    }
                }
            }
        }
    }
    }

    return 0;
}
