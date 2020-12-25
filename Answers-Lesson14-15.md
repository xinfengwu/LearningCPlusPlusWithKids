# 第14-15课 参考答案
## 复习题
1. D

2. B

3. A

4. B

## 编程练习
5.参考代码如下：

解法一、
```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
	const int MIMA_JIA=23434;//员工甲密码
	const int RENLIAN_JIA=1443;//员工甲人脸识别码
	const int ZHIWEN_JIA=3423;//员工甲指纹识别码
	
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
	const int MIMA_JIA=23434;//员工甲密码
	const int RENLIAN_JIA=1443;//员工甲人脸识别码
	const int ZHIWEN_JIA=3423;//员工甲指纹识别码
	
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
6.参考代码如下：

```cpp
#include<iostream>
#include<iomanip>
using namespace std;
int main()
{
    int a;
    int i;//偶数计数器
    int j;//奇数计数器

    i=j=0;//计数器初始化为0

    cin>>a;
     if(a%2==0)
     {
        cout<<"偶数"<<endl;
        i++;//偶数计数器累加
    }
    else
    {
        cout<<"奇数"<<endl;
        j++;//奇数计数器累加
    }
    
    cin>>a;
     if(a%2==0)
     {
        cout<<"偶数"<<endl;
        i++;
    }
    else
    {
        cout<<"奇数"<<endl;
        j++;
    }

    cin>>a;
    if(a%2==0)
    {
        cout<<"偶数"<<endl;
        i++;
    }
    else
    {
        cout<<"奇数"<<endl;
        j++;
    }

    cin>>a;
    if(a%2==0)
    {
        cout<<"偶数"<<endl;
        i++;
    }
    else
    {
        cout<<"奇数"<<endl;
        j++;
    }

    cout<<"偶数共"<<i<<"个，"<<"奇数共"<<j<<"个。"<<endl;

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
    float p1=0.7;//第一档电价
    float p2=0.8;//第二档电价
    float p3=1;//第三档电价
    float p4=2.1;//第四档电价

    float b1=360;//第一档用电量临界点
    float b2=468;//第二档用电量临界点
    float b3=720;//第三档用电量临界点

    float bill1 = p1*b1;//360度电的总电费
    float bill2 = bill1 + (b2-b1)*p2;//用468度电的总电费
    float bill3 = bill1 + bill2 + (b3-b2)*p3;//用720度电的总电费

	float bill;//总费用
	float ydl;//用电量
	
	cout<<"请输入用电量："<<endl;
	cin>>ydl;
	
	if(ydl<=b1)
		bill = ydl * p1;//用电量在360度以内
	else
		if(ydl<=b2)
			bill = bill1 + (ydl-b1)*p2;//用电量在360~468度以内
		else
			if(ydl<=b3)
				bill = bill2 + (ydl-b2)*p3;//用电量在468~720度以内
			else
				bill = bill3 + (ydl-b3) * p4;//用电量超过720度
				
    cout<<ydl<<"度电的电费为："<<bill<<"元。"<<endl;
    return 0;
}
```

