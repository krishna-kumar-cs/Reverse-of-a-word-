# Reverse-of-a-word-
#include<stdio.h>
#include<string.h>
int main()
{
    char str[50];
    puts("Enter a word to print it's reverse");
    scanf("%[^\n]s",str);
    int i = 0;
    int size = 0;
    while(str[i]!='\0'){
       size++;
       i++;
    }
    for(int i=0,j=size-1; i<j; i++,j--){
      char temp;
      temp   = str[i];
      str[i] = str[j];
      str[j] = temp;
    }
    puts("the reverse is");
    puts(str);
    return 0;
}