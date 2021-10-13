#include <stdio.h>



int primeno(int num);
void printPrime(int start, int end);



int main()
{
    int start, end;
    
    printf("Enter the starting and ending range of numbers: ");
    scanf("%d%d",&start, &end);
    
    
    printPrime(start, end);
    
    return 0;
}




void printPrime(int start, int end)
{
    printf("The prime number between %d to %d are: ", start, end);
    
    while(start<=end)
    {
        
        if(Primeno(start))
        {
            printf("%d, ",start);
        }
        
        start++;
    }
}




int Primeno(int num)   
{  
    int i;  
      
    for(i=2; i<=num/2; i++)    
    {    
          
        if(num % i == 0)    
        {  
            return 0;  
        }    
    }   
      
    return 1;   
}
