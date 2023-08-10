%{
#include<stdio.h>
%}
%%
[A-Z]+[\t\n] {printf("%s",yytext);}
. ;
%%
int main()
{
printf("\n enter the input:");
yylex();
}
int yywrap()
{
return 1;
}
