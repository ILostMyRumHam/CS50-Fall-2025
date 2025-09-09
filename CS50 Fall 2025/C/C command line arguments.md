```c
#include <stdio.h>
#include <cs50.h>

int main (main void)
{
	string answer = get_string("What's your name? ");
	printf("hello, %s/n", answer);
}
```

```c
#include <stdio.h>

#include <cs50.h>

int main(int argc, string argv[])

{

    if (argc == 2)

    {

    printf("hello, %s\n", argv[1]);

    }

    else

    {

        printf("hello, world\n");

    }

}
```
make greet 
./greet (input)

```c
#include <stdio.h>
#include <cs50.h>

int main(int argc, string argv[])
{
    for (int i = 0; i < argc; i++)
    {
        printf("%s\n", argv[i]);
    }
}
```

numbers are used to standartise what is wrong with a programme
0 - should not be used to indicate an error 

```c
#include <cs50.h>
#include <stdio.h>

int main(int argc, string argv[])

{

    if (argc != 2)

    {

        printf("Missing command-line argument\n");

        return 1;

    }

    printf("Hello, %s\n", argv[1]);

    return 0;

}
```