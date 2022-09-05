# Pic 16F887 Con Oscilador Interno

<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/16f887-Pic.png"  />

* Vdd: Positivo del microcontrolador
* Vss: Negativo del microcontrolador

### Codigo
```c
#include <16f887.h> //Nombre del microcontrolador
#fuses LP,nowdt  //para osciladores de 32KHz
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

### Compilar en Css Compiler
<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/Codigo-Imagen.png"  />

### Conectar el Pic al Pickit 
<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/Pickit3.jpg" width="1000" height="500" />

### Subir el archivo Hex al Pickit 
<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/Importar-Hex.png"  />

### Luego subir el programa al microcontrolador con "Write"
<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/Write-pickit.png"  />

### Conexion
<img src="https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/Circuito-En-Fritizing.png" />

### Funcionamiento
![](https://github.com/IDiegoUlises/Pic-Con-Oscilador-Interno/blob/main/Images/Pic-Con-Oscilador-Interno.gif)
