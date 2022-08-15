# octo-potato
#include<stdio.h>

#include<string.h>

int main()

{
    char str[10010];
    
    int i, j, n;
    
    scanf("%s", str);
    
    for (i=0; str[i]; i++)
    
    {
    
    if (str[i]=='?' || str[i]=='&')
    
    {
    
    for (j=i+1; str[j]!='='; j++)
    
    {
    
    printf ("%c", str[j]);
    
    }
    
    printf (": ");
    
    for(n=j+1; str[n]!='&' || str[n]!=0; n++)
    
    {
    
    printf("%c", str[n]);
    
    }
    
    printf ("\n");
    
    }



}

return 0;

}
