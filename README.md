# zuoye1
二柱子四则运算问题
//随机输出30个四则运算式
//2016/3/7;李营；20142930
#include<iostream>
using namespace std;

void main()
{

　　int n;
　　cout<<"请输入四则运算数的种类（1为整数，2为假分数）："<<endl;
　　cin>>n;
　　int a,b,c,d,y;
　　for(int i=0;i<30;i++)
　　{
　　　　a=rand()%100;
　　　　b=rand()%100;
　　　　y=rand()%4;
　　　　if(n==1)
　　　　{
　　　　　　if(b==0)
　　　　　　{
　　　　　　　　i--;
　　　　　　} 
　　　　　　else
　　　　　　{
　　　　　　　　cout<<i+1<<": ";
　　　　　　　　if(y==0)
　　　　　　　　{
　　　　　　　　　　cout<<a<<"+"<<b<<"="<<endl;
　　　　　　　　}
　　　　　　　　else if(y==1)
　　　　　　　　{
　　　　　　　　　　cout<<a<<"-"<<b<<"="<<endl;
　　　　　　　　}
　　　　　　　　else if(y==2)
　　　　　　　　{
　　　　　　　　　　cout<<a<<"*"<<b<<"="<<endl; 
　　　　　　　　}
　　　　　　　　else
　　　　　　　　{
　　　　　　　　　　cout<<a<<"/"<<b<<"="<<endl; 
　　　　　　　　}
　　　　　　 }
　　　　}
　　　　else if(n==2)
　　　　{
　　　　　　c=rand()%100;
　　　　　　d=rand()%100; 
　　 　　　  if(b>=a||d>=c)
　　　　　　{
　　　　　　　　i--;
　　　　　　} 
　　　　　　else
　　　　　　{
　　　　　　　　cout<<i<<": ";
　　　　　　　　if(y==0)
　　　　　　　　{
　　　　　　　　　　　　cout<<"("<<a<<"/"<<b<<")+("<<c<<"/"<<d<<")="<<endl;
　　　　　　　　}
　　　　　　　　else if(y==1)
　　　　　　　　{
　　　　　　　　　　　　cout<<"("<<a<<"/"<<b<<")-("<<c<<"/"<<d<<")="<<endl;
　　　　　　　　}
　　　　　　　　else if(y==2)
　　　　　　　　{
　　　　　　　　　　　　cout<<"("<<a<<"/"<<b<<")*("<<c<<"/"<<d<<")="<<endl; 
　　　　　　　　}
　　　　　　　　else
　　　　　　　　{
　　　　　　　　　　　　cout<<"("<<a<<"/"<<b<<")/("<<c<<"/"<<d<<")="<<endl;
　　　　　　　　}
　　　　　　}
　　　　}

}
