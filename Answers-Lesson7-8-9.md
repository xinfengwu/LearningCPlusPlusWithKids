# 第7-8-9课 参考答案
## 复习题
1. 符合规范：DF；不符合有：ABCE

2. ① #include<iomanip>

② int a,b

③ cin>>b

④ 5

⑤ a*b

⑥ 略

## 编程练习
3.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
  int a=10,b=3,c=7,t;
	t = a;
	a = b;
	b = c;
	c = t;

	cout<<"a="<<a<<endl<<"b="<<b<<endl<<"c="<<c<<endl;
  
  return 0;
}
```
4.	参考代码如下：
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	int a=56,b=54;
	
	cout<<setw(10)<<a<<endl;
	cout<<setw(4)<<"*"<<setw(6)<<b<<endl;
	cout<<"----------"<<endl;
	cout<<setw(10)<<a*b<<endl;
	
	return 0;
}
```
5.	参考代码如下：
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	int sumPages,avPages;
	
	cout<<"请输入总页数：";
	cin>>sumPages;
	cout<<"请输入平均每天月的的页数：";
	cin>>avPages;
	cout<<"读完这本书需要："<<sumPages/avPages<<"天。";
	return 0;
}
```

6.	参考代码如下：
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	int downloadSpeed,fileSize,downloadTime;
	int times=1024;
	
	cout<<"请输入下载速度（KB/s）：";
	cin>>downloadSpeed;
	cout<<"请输入要下载的文件大小（MB）：";
	cin>>fileSize;
	
	cout<<"以"<<downloadSpeed<<"KB/s的速度，下载"<<fileSize<<"MB的文件，需要"<<times*fileSize/downloadSpeed<<"秒。";

	return 0;
}

```
7.	参考代码如下：
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	int avCon,sumPersons,sumRice,Sumcon;
	int days = 30;
	int price = 1;
	
	cout<<"请输入每天每人平均消耗的大米量（以斤为单位）：";
	cin>>avCon;
	cout<<"该家庭的总人口数:";
	cin>>sumPersons;
	
	cout<<"该家庭共有"
		<<sumPersons
		<<"口人，平均每人每天消耗"
		<<avCon
		<<"斤大米，30天共消耗"
		<<days*sumPersons*avCon
		<<"斤，共需花费"
		<<days*sumPersons*avCon*price
		<<"元。";

	return 0;
}

```
