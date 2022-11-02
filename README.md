#include <stdio.h>
#include <stdlib.h>




float fahren(float celcius){
return celcius*1.8+32;

}

float celcius(float fahren){
return (fahren - 32) / 1.8;
}



int main (){


float celciusderece;
float fahrenderece;
char secenek;
char F;
char C;



printf("hangisini ogrenmek istersiniz?(F-C)\n");
scanf("%c",&secenek);


if(secenek=='F'){
printf("c degerini girin...\n");
scanf("%f",&celciusderece);
printf("%f celcius = %f fahrenheit",celciusderece,fahren(celciusderece));
}



else if(secenek=='C'){
   printf("f degerini girin...\n");
scanf("%f",&fahrenderece);
printf("%f fahrenheit = %f celcius",fahrenderece,celcius(fahrenderece));
}



else{
    printf("gecersiz secenek...\n");
}

}
