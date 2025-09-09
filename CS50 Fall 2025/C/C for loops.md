
```c
#include <stdio.h>

int main() {
	int i; // Declare i outside or inside the loop 
	init for (i = 0; i < 3; i++){  
	// i is initialized, condition checked, i incremented 
		printf("%d\n", i);
	} 
		printf("After loop, i is: %d\n", i);// i retains its value after loop 
		return 0; 
}
```

Nested for loop


```c
#include <stdio.h>

  

int main(void){

    const int row_limit = 3;

    const int col_limit = 5;

    for (int row = 0; row < row_limit; row++){

        for (int col = 0; col < col_limit; col++){

            printf("#");

        }

        printf("\n");

    }

}
```