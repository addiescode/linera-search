# linera-search
linear search with multiple same numbers

#include<stdio.h>
int main ()
{

  int a[10], n, i, search, count = 0;

  printf ("Enter the number of elements in array\n");
  scanf ("%d", &n);
  printf ("Enter the %d array elements", n);
  for (i = 0; i < n; i++)
    {
      scanf ("%d", &a[i]);
    }
  printf ("Enter the number to search\n");
  scanf ("%d", &search);
  for (i = 0; i < n; i++)
    {
      if (a[i] == search)
	{
	  printf ("\n%d found at location %d", search, i + 1);
	  count++;
	}
    }
  if (count == 0)
    {
      printf ("\n%d is isnt in array\n", search);
    }
  else
    {
      printf ("\n%d is present %d times in array", search, count);
    }

  return 0;
}
