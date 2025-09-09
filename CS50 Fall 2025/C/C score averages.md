Source: https://www.youtube.com/watch?v=Y8qnryVy5sQ&t=2849s&ab_channel=CS50
```c
#include <stdio.h>

int main (void)
{
	int score1 = 72;
	int score2 = 73;
	int score3 = 33;

	// Print average 
	printf("Average: %f\n", (score1 + score2 + score3) / 3.0);
}
```
+ While this programme works, it is not good design - if additional scores are added, new variables have to be added and the print statement has to be adjusted
→ this can be solved using arrays

In an array, all of the data is of the same datatype

```c
#include <stdio.h>

int main (void)
{
	int scores [3];
	scores[0] = 72,
	scores[1] = 73,
	scores[2] = 33,

	// Print average 
	printf("Average: %f\n", (scores[0] + scores[1] + scores[2] / 3.0);
}
```
+ 0, 1, 2, 3 → indexing - technically one variable 

→ replacing repeating variable with a for loop 

```c
#include <stdio.h>
#include <cs50.h>

int main (void)
{
	int scores [3];
	for (int i = 1, i < 3; i++)
	{
		scores[i] = get_int("Score: ");
	}

	// Print average 
	printf("Average: %f\n", (scores[0] + scores[1] + scores[2]) / 3.0);
}
```

```c
// Averages three numbers using an array, a constant, and helper function 

#include <stdio.h>
#include <cs50.h>

// Constant 
const int N = 3;
// Prototype
float average(int length, int array[]);

int main(void)
{
	// Get scores
	int scores [N];
	for (int i = 0, i < N; i++)
	{
		scores[i] = get_int("Score: ");
	}

	// Print average 
		printf("Average: %f\n", (scores[0] + scores[1] + scores[2]) / (float) N);
}

float average(int average, int array[])
{
	// Calculate average
	int sum = 0;
	for (int i = 0, i < length; i++)
	{
		sum += array[i];
	}
	return sum / (float) length;

}

```
→ sometimes it is good to include constants at the beginning, outside of functions