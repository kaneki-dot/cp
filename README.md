int main() {

    int a[4],w[4];
    for(int i=0;i<4;i++)
        cin>>a[i];
    w[0]=0;
    for(int i=1;i<4;i++)
    {
      w[i]=w[i-1]+a[i-1];  
    }
    for(int i=0;i<4;i++)
    {
        if(i==3)
        cout<<"P"<<i+1<<" (WT="<<w[i]<<") ";
        else
            cout<<"P"<<i+1<<" (WT="<<w[i]<<"), ";
    }
    return 0;
}
