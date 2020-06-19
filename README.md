# Insertion-Sort
#include <stdio.h>


void insertionsort(int array[]){

int i,j,temp;

    for (size_t i = 1; i < 10; i++)
    {
         temp = array[i];

        j = i - 1;

        while (j >= 0 && array[j] > temp)
        {
             array[j + 1] = array[j];

            j -= 1;

         }

        array[j + 1] = temp;
    
    }



}



int main(){

printf("INSERTİON SORT\n\n\n");

int array[10] = {10,2,3,5,6,19,59,11,32,42};

insertionsort(array);

for (int i = 0; i < 10; i++)
{
    printf("%d ",array[i]);
}


    return 0;
}


