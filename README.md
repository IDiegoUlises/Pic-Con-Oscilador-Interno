# Pic 16F887 Con Oscilador Interno

<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/16f887-Pic.png"  />

* Vdd: Positivo del microcontrolador
* Vss: Negativo del microcontrolador

### Codigo
```c
#include <16f887.h> //Nombre del microcontrolador
#fuses LP,nowdt  //para osciladores de de 32KHz
#use delay(internal=32KHz) //Internal le dice que utilizara el oscilador interno

void main()
{
   while(true)
   {  
      output_high(pin_c0); //Enciende el led
      delay_ms(1000); //Espera de 1 segundo
      output_low(pin_c0); //Apaga el led
      delay_ms(1000); //Espera de 1 segundo
   }
}
```
