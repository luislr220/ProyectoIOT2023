# Caja fuerte con sensores

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
- Como usuario quiero poder visualializar el estatus de mi seguridad desde el celular 
- Como usuario quiero poder abrir la caja fuerte a distancia si lo requiero
- Quiero poder tener los datos de humedad desde mi celular
- Saber si alguien intenta abrir la caja fuerte
- que suene el buzzer si alguien intenta abrirla


## Tabla de historias de usuario
| Id  | Historia de usuario  |Prioridad |Estimación|Como probarlo | Responsable |
|---|---|---|---|---|---|
| 1  |Quiero ver como se encuentra mi caja fuerte sin importar donde me encuentre| Alta  | 1 mes | mqqt | por el equipo |
|  2| Quiero abrir la caja fuerte desde mi celuar en dado caso de que se requiera y yo no este presente| Media  | 2 semanas |mqqt y un celular|Por el equipo|
|  3 |Quiero saber el estado de mi caja| Media  | 1 semanas |Probando el sensor de humedad |Por el equipo|
|  4 | Yo como usuario quiero poder escuchar una alerta de luz y sonido cuando una puerta en especifico se abierta o cerrada|Alta|2 semanas|Probando el sensor de movimiento con el buzzer|Por el equipo|


## Prototipo en dibujo
- https://drive.google.com/file/d/1OgpiTpNm4uELDASEXitZ8KS-C9Qwsw3S/view?usp=drivesdk


