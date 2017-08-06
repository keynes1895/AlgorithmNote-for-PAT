```c++
#include<cstdio>
const int minn = 3;
const int maxn = 20;
int main(){
	int n,i;
	char cha;
	int col,row;
	scanf("%d %c",&n,&cha);
	if(n > minn && n < maxn){
		col = n;
		if(col % 2 == 1)
		row = col / 2 + 1;
		else row = col / 2;
	}
	for(i = 0; i < col; ++i){
		printf("%c",cha);
	}
	printf("\n");
	for(i = 2; i < row; ++i){
		printf("%c",cha);
		for(int j = 0; j < col - 2; ++j){
		printf(" ");
		}
		printf("%c\n",cha);
	}	
	for(i = 0; i < col; ++i){
	printf("%c",cha);
	}
	return 0;
} 
```

![Markdown](http://i2.bvimg.com/1949/9fe7a9ce8eb1f92e.png)