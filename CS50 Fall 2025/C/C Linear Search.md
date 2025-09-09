
```c
#include <cs50.h>
#include <stdio.h>

int main (void)
{
	int numbers[] = {20, 500, 10, 5, 100, 1, 50};

	int n = get_int("Number: ");
	for (int i = 0; i < 7;; i++)
	{
		if (numbers[i] == n)
		{
			printf("Found\n");
			return 0;
		}	
	}
	printf("Not found\n");
	return 1;
}
```

```c
#include <cs50.h>
#include <stdio.h>
#include <string.h>

int main (void)
{
	string strings_array[] = {"battleship", "boot", "cannon", "iron", "thimble"};
	// Hard-coding number of values in the array - not good practice, change later 
	string s = get_string("String: ");
	for (int i = 0; i < 5, i++)
	{
		if (strcmp(string_array[i], s) == 0)
		{
			printf("Found\n");
			return 0;
		}
	}
	printf("Not found\n");
	return 1;
}
```

Cannot compare strings with == in c
as in
```c
if (strings_array[i] == s)
```

Can compare integers, longs etc.

Here the strcmp() function is used instead (string compare)