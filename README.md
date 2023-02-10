# ProjectsIoT2022

## Integrantes
- Luis Armando Largo Ramirez
- Josue Omar Nuñez Godinez
- Omar Zuñiga Abundis
- Juan David Lara Robles

## Objetivo general
Nuestro objetivo con este proyecto es poder garantizar la seguridad de las pertenencias de las personas no solo en un intento de robo si no tambien por cosas naturales como podria ser que el interior de la caja fuerte este muy humedo.
### Objetivos específicos
- El programa detectará la humedad de la caja fuerte.
- Se abrirá automaticamente la caja si detecta que humedad sobrepasando el limite para evitar el daño.
- Sonara un buzzer en caso de que la caja se habra sin autorización del propietario.


## Tabla de Software utilizado
|id | Sofware  | Version  |Tipo   
|---|---|---|---| 
| 1 | Arduino IDE  |2   |   2|   Freeware 
| 2| Mosquitto  |   5.0, 3.1.1  | Freeware  | 
| 3| NODE-RED  |  3.0 | Freeware  | 


## Tabla con el hardware utilizado

| Id  |Componente   | Descripción | Imagen | Cantidad |Costo Total |
|---- |------------ |------------ |------- | -------- | ---------  |
| 1   |   Esp32   |La placa ESP32 está basada en el modulo ESP32-WROOM-32 que trae integrado Wi-Fi, Bluetooth y BLE (Bluetooth Low Energy).| ![image](https://user-images.githubusercontent.com/106614070/214468798-4a2ca8ec-510a-43d5-82c8-5b31b9dbc32a.png)| 1 | $150|
| 2   | Raspberry Pi 4|Ésta nueva versión incluye 4GB de memoria RAM DDR4 y permite conectar dos monitores 4K a la vez a través de dos puertos micro HDMI. Además de dos puertos USB 2.0, la Raspberry Pi 4 también tiene dos puertos USB 3.0 que hacen que las transferencias de datos sean mucho más rápidas a través de USB.|<img  src= "https://user-images.githubusercontent.com/106614070/214469274-f2f560df-0885-4fcd-95ee-3a434b0d50a4.png" width="200" height="200" />|1|$3250|
| 3   |Sensor De Movimiento|Es usado para la detección de movimiento cuenta con una excelente sensibilidad, fiabilidad y estabilidad, puede ser ampliamente utilizado en muchos tipos de equipos eléctricos de inducción automática.|<img  src= "https://user-images.githubusercontent.com/106614070/214469755-bf5b4626-8ed1-402e-b3a0-162a04ec8f0d.png" width="200" height="200" />|1| $47|
| 4   |Buzer|WE un pequeño transductor capaz de convertir la energía eléctrica en sonido.|<img  src= "https://user-images.githubusercontent.com/106614070/214469963-c4d8d5b9-03d3-48ae-ba49-d985c0ca5646.png" width="200" height="200" />| 1| $25 |
|   5| Sensor Dht11| El DHT11 es un sensor digital de temperatura y humedad relativa de bajo costo y fácil uso. Integra un sensor capacitivo de humedad y un termistor para medir el aire circundante, y muestra los datos mediante una señal digital en el pin de datos (no posee salida analógica) |<img  src= "https://http2.mlstatic.com/D_NQ_NP_2X_638466-MLM29979046786_042019-F.webp" width="200" height="200" />  |  1 | $50|
|   6|Leds| Un diodo LED es un dispositivo que permite el paso de corriente en un solo sentido y que al ser polarizado emite un haz de luz. Trabaja como un diodo normal pero al recibir corriente eléctrica emite luz.|!<img  src= "https://user-images.githubusercontent.com/106614070/193472526-db15e319-4390-4c06-8c58-0bf9736962b8.png" width="200" height="200" />| 3| $45 | 
|   8|  Protoboard| Es una tablilla de pruebas, que cuenta con 830 perforaciones divididas en filas horizontales y columnas verticales para realizar conexiones eléctricas, puedes conectar cualquier elemento electrónico para realizar prototipos, prácticas y simulaciones de circuitos electrónicos| <img  src= "https://user-images.githubusercontent.com/106614070/193472640-0e12c7f3-c74e-4f16-9562-9829b3982a2d.png" width="200" height="200" />|1|$52 |
|   8| Cables Jumpers|  Un cable puente para prototipos (o simplemente puente para prototipos), es un cable con un conector en cada punta (o a veces sin ellos), que se usa normalmente para interconectar entre sí los componentes en una placa de pruebas. | <img  src= "https://user-images.githubusercontent.com/106614070/193472720-f2f6cb77-627d-4a3d-acd6-4f6ec8571d7f.png" width="200" height="200" />|1  |$150|
|  9 | Motor A Pasos|Un motor a pasos convierte los impulsos digitales en pequeños pasos de movimiento en una dirección. Se mueve sólo un paso a la vez, pero puede girar indefinidamente cada vez que se repita la secuencia de pasos.|  <img  src= "https://user-images.githubusercontent.com/106614070/214470613-e65f5ec5-e2bb-438e-a316-3f768d051c45.png" width="200" height="200" />|1 |$66.0 |




## Epicas del proyecto (Minimo debe de haber una épica por integrante de equipo)
- Quiero poder abrir la puerta desde cualquier lugar del mundo donde me encuentre  
- Como usuario quiero poder visualializar el estatus de mi seguridad desde el celular 
- Como usuario quiero poder ver el clima en una pantalla lcd y como el clima 


## Tabla de historias de usuario
| Id  | Historia de usuario  |Prioridad |Estimación|Como probarlo | Responsable |
|---|---|---|---|---|---|
| 1  |Quiero poder abrir la puerta desde cualquier lugar del mundo donde me encuentre| Alta  | 3 semanas | Con conexion mqqt y un celular | Cesar Alegandro Ordoñez Osorio |
|  2| Como usuario quiero poder ver el clima en una pantalla lcd y como el clima   | Media  | 2 semanas | Probando mando los valores que mandan los se nsores ala pantalla | Cruz Estrella Juárez Soto |
|  3 | Yo como usuario quiero poder visualizar el estatus de la puerta desde mi celular en una aplicación web responsiva   | Media  | 3 semanas | Probando mando los valores que mandan los sensores ala aplicacion web | Cruz Estrella Juárez Soto |
|  4 | Yo como usuario quiero poder escuchar una alerta de luz y sonido cuando una puerta en especifico se abierta o cerrada  | Alta  | 2 semanas    | Con las aplicacion web resposiva probando que el seguro abre y cierra correctamete  | Angel Gerardo Velazquez Salazar |
|  5 | Yo como usuario quiero poder visualizar el estatus de mi seguro inteligente en una pantalla lcd además de visualizar el clima del momento en el que me encuentro de salida de una habitación en especifico  | media  | 2 semanas    | Captando los valores que viene de los sensores y pasandolos ala pantalla  | Angel Gerardo Velazquez Salazar |
| 1  |Como usuario de la cerradura inteligente quiero poder  asegurar la puerta cada 5 minutos de no haber detectado presencia humana| Alta  | 3 semanas | Reciviendo los valores deuna sensor mandar indicaciones al motor y activar la seguridad | Cesar Alegandro Ordoñez Osorio |


## Prototipo en dibujo
- Coloca la fotografia de tu prototipo dibujado a lapiz


