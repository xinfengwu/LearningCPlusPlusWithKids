# 第5-6课 参考答案
## 复习题
1. a) X=30; b) X=27;  c) X=1, Y=1;  d) X=2,Y=7

2. 输出:
t=5,
a=5,
b=5

## 编程练习
3.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
	int biaoMianJi=100,ceMianJi=80,diMianJi;
	diMianJi=(biaoMianJi-ceMianJi)/2;
	cout<<"一个底的面积为：" 	<<diMianJi<<endl;
	return 0;
}
```
4.	参考代码如下：
```cpp
#include<iostream>
using namespace std;
int main()
{
	/*
	10.28   -30 	+30
	10.29   -60 	+30
	10.30   -120 	+30
	10.31   -240    +30
	11.1    -480    +30
	11.2

	*/
	int jiShu=30;		//第一天采摘数量
	int xinZeng=0;    //每天新成熟的辣椒数量
	int shengYu;	//当天剩余的成熟辣椒数量
	
	//10.28
	xinZeng +=30;
	jiShu *=1;

	//10.29
	xinZeng +=30;
	jiShu *=2;

	//10.30
	xinZeng +=30;
	jiShu *=2;

	//10.31
	xinZeng +=30;
	jiShu *=2;

	//11.1
	xinZeng +=30;
	jiShu *=2;
	
	shengYu = 1000 - jiShu + xinZeng;
	
	cout<<"11月2日（采摘之前）农场的菜园里还有"<<shengYu<<"个成熟的辣椒"<<endl;

	return 0;
}

```
5.	参考代码如下：
```cpp
略
```

