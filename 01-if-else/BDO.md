#include <stdio.h>
void main ()
{
	int shiba;
	int GP;
	printf("silver shiba: ");
	scanf("%d", &shiba);
	printf("GP shiba: ");
	scanf("%d", &GP);
	if (shiba >= 500 && shiba <= 600 && GP == 0){
		printf("White grade\n");
	}
	else if (shiba >= 601 && shiba <= 700 && GP == 0){
		printf("Green grade\n");
	}
	else if (shiba >= 701 && shiba <= 800 && GP == 0){
		printf("Blue grade\n");
	}
	else if (shiba >= 801 && shiba <= 900 && GP == 0){
		printf("Red grade\n");
	}
	else if (shiba >= 901 && shiba <= 1000 || GP == 1){
		printf("Golden grade\n");
	}
	else if (shiba >= 2000 || GP >= 2){
		printf("Rare grade\n");
	}
	else{
		printf("silver is not enough\n");
	}
	}