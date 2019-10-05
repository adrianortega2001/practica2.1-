# practica2.1-
No supe como hacerle para repetir el menú 
/*practica2
Adrian ortega Perez
*/
#include<stdio.h>
#include<conio.h>
int main(void){
    float a;
    float b;
    float c;
    char repetir;
do{
printf("1.Suma\n");
printf("2.Resta\n");
printf("3 Multiplicacion\n");
printf("4 Division\n");
printf("Introduce 1 para la suma\n");
printf("Introduce 2 para la resta\n");
printf("Introduce 3 para la multiplicacion\n");
printf("Introduce 4 para la division\n");
int opt;
scanf("%d",&opt);
printf("Introduce la primer cantidad:");
scanf("%f",&a);
printf("Intropduce la segunda cantidad:");
scanf("%f",&b);
switch(opt){
case 1:
    c=a+b;
    printf("El resultado es %f",c);
    break;
case 2:
    c=a-b;
    printf("El resultado es %f",c);
    break;
case 3:
    c=a*b;
    printf("El resultado es %f",c);
    break;
case 4:
        while(b==0){
                printf("El segundo valor debe ser distinto de cero \n");
                printf("Introduce la segunda cantidad:");
        scanf("%f",&b);
        }
        c=a/b;
        printf("El resultado es %f",c);
            break;
    default:
        printf("Opcion invalida");
}
printf("Desea hacer otra operacion? S N  :");
repetir=getche();
}
while(repetir=="s" || repetir=="S");
}
