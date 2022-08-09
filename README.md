/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>

int main(int argc, char** argv) {
    float salario, inss, ir, sal_liquido;
    
    printf("digite seu lario bruto");
    scanf("%f", &salario);
    
	if(salario <=1903.98)
    {
        inss =salario * 0.00;
    }
    else
    if(salario >= 1903.99 && salario <= 2826.65)
    {
        inss = salario * 0.07;
    }
    else
     if(salario >= 2826.66 && salario <=  3751.05 )
    {
        inss = salario * 0.15;
    }
    else
     if(salario >= 3751.06 && salario <= 4664.68 )
    {
        inss = salario * 0.22;
    }
    else
    if(salario >4664.68)
    {
        inss =salario * 0.27;
    }
    
    sal_liquido = (salario - inss) -ir;
    
    printf ("\n in desconto  inss: %f\n", inss);
    
    printf("\n sal_liquido inss: %2.f\n", sal_liquido);
    
    return 0;
}
