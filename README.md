#include <stdio.h>
#define LENGTH 4
int main()
 {
	int i,j,temp,a[LENGTH];
	printf("input LENGTH numbers:\n");
	for (i=0;i<LENGTH;i++){
		scanf("%d",&a[i]);
	}
	for(i=0;i<LENGTH-1;i++){
		for(j=0;j<LENGTH-1-i;j++){
			if(a[j]>a[j+1])
			{temp=a[j];a[j]=a[j+1];a[j+1]=temp;} 
		}
	}
	for(i=0;i<LENGTH;i++){ 
		printf("%d ",a[i]);
	}
	return 0;
} 


