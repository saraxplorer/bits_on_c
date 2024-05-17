To be able to modify a string directly, It needs NOT to be a const. If it is, it cannot be directly updated. 
For example here I am modifying the string because it is not a const 
``` c
int main(int argc, char **argv)
{
	if (argc == 2)
	{
		int i = 0;
		while (argv[1][i] != '\0')
		{
			if (argv[1][i] >= 'A' && argv[1][i] <= 'Z')
			{
				argv[1][i] = 'Z' - argv[1][i] + 'A';
				write(1, &argv[1][i], 1);
			}
```
If the input  was const char **argv, it would not be possible. 
Here I make lowercase but with the help of a char that will store the changed value
``` c
int ft_atoi_base(const char *str, int str_base)
{
  int result = 0;
  int sign = 1;
  int digit;
  int i = 0;
  char c;

  while (str[i] != '\0')
  {
    
    if (str[0] == '-')//handle minus sign
    {
       sign = -1;
       i++;
    }
    if (str[i] >= 'A' && str[i] <= 'Z') //Handle uppercase
        c = c + ('a' - 'A');//make all lowercase, and store it in a char, because we 
                          //cannot modify a const str
      i++;
  }
}
```
