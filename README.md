# -
全局变量的屏蔽
#include "stdafx.h"
#include<iostream>
using namespace std;

int i;  //全局变量，文件作用域
int _tmain(int argc, _TCHAR* argv[])
{
	i=7; //为全局变量赋值
	{
		int i;
		i=5;
		cout<<"i="<<i<<endl; //输出5

	}
	cout<<"i="<<i<<endl; //输出7
	return 0;
}

  
