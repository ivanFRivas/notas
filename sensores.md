# sensores

#arduino

1. Sensores Ultrasónicos (HC-SR04)

Es la opción más clásica, económica y fácil de programar para maquetas.

    ¿Cómo funciona? Colocas un sensor en el extremo de cada calle (por ejemplo, apuntando hacia donde se acumulan los "autos"). A medida que los cubos se van acumulando y tapan el carril, el sensor mide la distancia y sabe qué tan llena está la fila.


2. Sensor de Luz Infrarroja (TCRT5000 o Barreras Infrarrojas)

Excelente si quieres un conteo más preciso de "cuántos autos pasan" o detectar presencia exacta en puntos clave.

    ¿Cómo funciona? Puedes poner los sensores emisor/receptor cruzando la calle a ras de suelo o empotrados en la pista. Cuando un cubo pasa por encima, interrumpe el haz de luz (o el sensor reflectivo rebota en el fondo).


1. Sensores Ópticos / Infrarrojos (Ideales para maquetas)

Estos sensores detectan la presencia de un objeto cercano reflejando luz infrarroja o interrumpiendo un haz.

Sensor de obstáculos infrarrojo (KY-033 o similar con potenciómetro):

    Cómo funciona: Emite un haz de luz infrarroja y detecta si rebota en un objeto. Puedes colocar varios a lo largo de los carriles embutidos en la calle o a los lados.

2. Sensores Ultrasónicos (HC-SR04)

Miden la distancia rebotando ondas de sonido.

    Cómo funciona: Si colocas un sensor ultrasónico al inicio o final de cada sentido de la calle apuntando hacia los autos (cubos), el sensor medirá qué tan cerca está el obstáculo. Si hay muchos autos acumulados, la distancia medida será menor.


3. RFID (Identificación por Radiofrecuencia) - Opción Avanzada y Creativa

Si quieres darle un toque muy tecnológico a tu maqueta:

    Cómo funciona: Puedes poner una pequeña etiqueta RFID (sticker) debajo de cada cubo de auto y un lector RFID (como el RC522) debajo de la calle del crucero.

    Ventaja: El sistema no solo sabría cuántos autos hay, sino incluso qué tipo de vehículo es (si diferencias los cubos con tags distintos, por ejemplo, un autobús o una emergencia).

4. Cámaras o Visión Artificial (Alternativa externa a Arduino)

    Mención honorífica: Aunque Arduino Uno estándar no tiene la potencia para procesar video, podrías usar una cámara económica como Pixy2 o conectar una ESP32-CAM para procesar
    la imagen externamente y enviar la orden a tu Arduino principal vía serial o Wi-Fi.

    Ideal para: Simular una cámara de tráfico real, aunque para una maqueta con cubos fijos o simples, los sensores infrarrojos o ultrasónicos son mucho más prácticos y estables.:w





