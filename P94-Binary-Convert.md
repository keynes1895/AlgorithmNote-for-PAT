```c++
#include<cstdio>
int main(){
	int A, B;
	int sum, D;
	int i = 0;
	int ans[31];
	scanf("%d%d%d", &A , &B, &D);
	sum = A + B;
	do{
		ans[i++] = sum % D;
		sum = sum / D;
	} while(sum != 0); 
	for(int j = i - 1; j >= 0; j--) {
		printf("%d",ans[j]);
	}
	return 0;
} 
```

![Markdown](http://i1.bvimg.com/1949/453c7a35af15c644.png)