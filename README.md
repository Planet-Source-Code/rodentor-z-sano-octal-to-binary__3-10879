<div align="center">

## Octal To Binary


</div>

### Description

Converting
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Rodentor Z\. Sano](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/rodentor-z-sano.md)
**Level**          |Beginner
**User Rating**    |2.3 (7 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/rodentor-z-sano-octal-to-binary__3-10879/archive/master.zip)





### Source Code

```
#include<stdio.h>
#include<conio.h>
#include<string.h>
#define MAX 100
main(){
char bin[20];
int dec,temp;
int i=0;
	clrscr();
		printf("Enter octal number: ");
		scanf("%d", &dec);
		temp=dec;
		int a=0;
		do{
			a=temp%8;
			if(a==0){
				bin[i++]='0';
			}else if(a==1){
				bin[i++]='1';
			}
			dec/=8;
			temp=dec;
		}while(dec>0);
		printf("\n");
		printf("Binary value is ");
		for(int j=i;j>=0;--j){
			printf("%c", bin[j]);
		}
	getch();
	return 0;
}
```

