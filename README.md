#include<iostream>
#include<time.h>
using namespace std;
int main()
{
int hr,min,secn=0;
while(1)
{
system("clear"); 
cout<<hr<<min<<secn;
fflush(std);
secn++;
if(secn==60)
{
min+=1;
secn=0;
}
if(min==60)
{
hr+=1;
min=0;
}
if(hr==24)
{
hr=0;
min=0;
secn==0;
}
sleep(1);
}
}
