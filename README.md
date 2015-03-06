# mario
mario pirámide

/******************************
* mario.c
* Rafael Aaron Torres Teista 
*djrafazx@gmail.com
*
* Recrear una media-piramide de mario background
*********************************************/
#include <stdio.h>

int main(void)
{	
	int altura, i, j;
	
	do	
	{ // Se obtiene el valor de la altura 

	   printf("Altura: ");
	   scanf("%d", &altura);

	}
	while(altura <= 0 || altura > 23 );
	
	printf("\n");
	//Construcción de la piramide
	for(i = 1; i < altura; i++)
	{	 
		int espacio, space; 
		espacio = altura - i;
		// espacio de la piramide altura - pasos
		for(space = 1; space < espacio; space++)
		{	
			
			printf(" ");
		}		
		
		// filas de bloques 
		for(j = 0; j <= i ; j++)
		{  
		  
		   printf("#", j + 2);
		   
		}
		
		printf("\n"); // nueva linea
	}

	return 0;	
}
