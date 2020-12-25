# 第14-15课 参考答案
## 复习题
1. D

2. B

3. A C

4. B

## 编程练习
5.	参考代码如下：

解法一、
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	const int MIMA_JIA=23434;
	const int RENLIAN_JIA=1443;
	const int ZHIWEN_JIA=3423;
	
	int mima,renlian,zhiwen;
	cout<<"请依次输入密码、人脸识别码和指纹识别码：";
	cin>>mima>>renlian>>zhiwen;
	
	if(mima==MIMA_JIA)
		if(renlian==RENLIAN_JIA)
			if(zhiwen==ZHIWEN_JIA)
				cout<<"欢迎回来！";
				
	if(mima!=MIMA_JIA)
		cout<<"密码错误，请重试！";
		
	if(renlian!=RENLIAN_JIA)
		cout<<"人脸识别错误，请重试！";

	if(zhiwen!=ZHIWEN_JIA)
		cout<<"指纹识别错误，请重试！";

	return 0;
}
```

解法二、
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	const int MIMA_JIA=23434;
	const int RENLIAN_JIA=1443;
	const int ZHIWEN_JIA=3423;
	
	int mima,renlian,zhiwen;
	cout<<"请依次输入密码、人脸识别码和指纹识别码：";
	cin>>mima>>renlian>>zhiwen;
	
	if(mima==MIMA_JIA)
		if(renlian==RENLIAN_JIA)
			if(zhiwen==ZHIWEN_JIA)
				cout<<"欢迎回来！";
			else
				cout<<"指纹识别错误，请重试！";
		else
			cout<<"人脸识别错误，请重试！";
	else
		cout<<"密码错误，请重试！";

	return 0;
}
```
6.	参考代码如下：
```cpp

```

7.	参考代码如下：
```cpp

```

