# 第3-4课 参考答案
## 复习题
1. 声明变量i,m,n

2. 给变量i赋值0；给变量m赋值2；给变量n赋值5

3. 不可以。变量的使用要遵循要声明后赋值原则。

4. 6    n=m+n;

5. 运行结果：
```
12
3
```

## 编程练习
6.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
	int m,n,sum;
	m=10;
	n=12;
	sum=m*n;
	cout<<"李叔叔送给敬老院"<<sum<<"个菜椒。" ; 
	return 0;
}
```
7.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
	int m,n,sum;
	m=4;
	n=10;
	sum=m*n;
	cout<<"小明编写的程序总共有"<<sum<<"个字符。" ; 
	return 0;
}
```

8.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
	int m,n,sum;
	sum=1056; 
	m=30;
	n=sum/m;
	cout<<"每箱"<<n<<"个。";
	return 0;
}
```
9.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
  int sum=132,m=72,n=0,l=5,k=9;
  n=(sum-m)/l;
  cout<<"看了5天后还剩72页，平均每天看了"<<n<<"页。"<<endl;
  
  cout<<"从第6天起，平均每天要看"<<m/9<<"页。"<<endl;  
  return 0;
}
```
