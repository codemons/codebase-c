[Display Patterns](http://codemons.com/codebase/)
===============

Programs to display patterns like the right angled triangle, diamond etc.

### CODE
```c
int main()
{
    int row, c, n;
    char ch[4];

    printf("Enter the number of rows in triangle :: ");
    scanf("%d",&n);
    printf("Enter a character to be printed :: ");
    scanf("%s",&ch);

    for ( row = 1 ; row <= n ; row++ ) {

        for ( c = 1 ; c <= row ; c++ ) {
            printf("%c", ch[0]);
        }

        printf("\n");
    }

    return 0;
}
```

### RESULT
```
Enter the number of rows in triangle :: 6
Enter a character to be printed :: a
a
aa
aaa
aaaa
aaaaa
aaaaaa
```

### CODE
```c
int main()
{
    int row, c, n;
    char ch[4];

    printf("Enter the number of rows in triangle :: ");
    scanf("%d",&n);
    printf("Enter a character to be printed :: ");
    scanf("%s",&ch);

    for ( row = 1 ; row <= n ; row++ ) {

        for ( c = 1 ; c <= n-row ; c++ ) {
            printf(" ");
        }

        for ( c = 1 ; c <= row ; c++ ) {
            printf("%c", ch[0]);
        }

        printf("\n");
    }

    return 0;
}
```

### RESULT
```
Enter the number of rows in triangle :: 6
Enter a character to be printed :: a
     a
    aa
   aaa
  aaaa
 aaaaa
aaaaaa
```

:+1: