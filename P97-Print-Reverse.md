```c++
#include <cstdio>
#include <cstring>
const int maxn = 90;
int main() {
	char str[maxn];
	gets(str); 
	int len = strlen(str);
	int row = 0, col = 0;
	char ans[maxn][maxn];
	for(int i = 0; i < len; i++) {
		if(str[i] != ' ') {
			ans[row][col++] = str[i];
		}else {
			ans[row][col] = '\0';
			row++;
			col = 0; 
		}
	}
	for(int i = row; i >= 0; i--) {
		printf("%s",ans[i]);
		if(i > 0) {
			printf(" ");
		}
	}
	return 0;
} 
```

![Markdown](http://i1.bvimg.com/1949/e0db2db6a584cddc.png)