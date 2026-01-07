# tallerdaisy
taller dictado entre 5,7 y 9 de enero utilizando el microcontrolador de audio daisypod de electrosmith


## jornada 7 de enero en LID

### repaso del día lunes

- el lunes terminamos la clase presentando el código del procesamiento de audio
- en librería de daisy vienen bloques de procesamiento de audio, son 3 principales: delayline, oscillator oscilación en tiempo real y  onepole, es la clase de daisy, nos permite??
- actúan dentro del ciclo for
- dónde modificar, qué es lo que quiero modificar, debería comentar el código para ir desglosando ideas
- filtros de pasabaja y pasaalta
- en la línea
- función para actualizar valores de perillas, botones, leds
- 2 tipos de señales de control, trigger y gate, un trigger es una instrucción instantánea
- un gate es una señal continua, como un 1 o un 0 continuos
- necesitamos crear una variable que guarde el estado del filtro
- es parecido a cuando necesitaba establecer un valor en un estado del motor y otro valor en el otro estado del motor (máquina asombrosa referencia)

### perillas

- perilla 1 la definimos para controlar el tiempo, valor mínimo y máximo del tiempo que vamos a usar
- perilla 2 cambia valor de feedback (cuantass repeticiones escucharemos de delay) y frecuencia del filtro
- poder usar una perilla para cambiar 2 estados distintos, ej hacia la izq cambio el filtro y hacia la derecha cambio la saturación, cuando hago una u otra, la que no está siendo activada no se ve afectada
- poner mouse arriba de las funciones me permite ver la info de la función
- el void update encoder define los valores máximos y mínimos del encoder, si llega a 50 que es el máximo no va a pasar más allá de eso, si llega a 0 lo mismo

### leds

- el encoder no posee indicadores de posición por lo cuál se fijó que en 25 (la mitad del rango) el led es morado
- puedo indicar de qué color quiero cada led según el rango del encoder
