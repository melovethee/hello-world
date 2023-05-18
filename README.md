# hello-world
hello world
//输出101到200的所有素数
#include<stdio.h>
#include<math.h>
int main()
{
	int m ,k,i,h=0;
	for (m = 101; m <= 200; m++)
	{
		int leap = 1;
		k = sqrt((m + 1));
		for (i = 2; i <= k; i++)
		{
			if (m % i == 0)
			{
				leap = 0;
				break;
			}
		}
			if (leap)
			{
				printf("%4d", m);
				h++;
				if (h % 10 == 0)
				{
					printf("\n");
				}
			}
		
	}
	return 0;
}
