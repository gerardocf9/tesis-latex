# Análisis de Vibración

Se conoce como análisis de vibración, al conjunto de técnicas que permiten
obtener información de un equipo, a partir de sus vibraciones. Es una de las
técnicas más usadas en el mantenimiento predictivo de equipos mecánicos, debido
a que es un proceso poco invasivo y de bajo costo. El análisis de vibración
permite diagnosticar fallas de forma temprana, así como detectar señales
prematuras de desgaste.

Según Girdhar (2004) el análisis de vibración nos permite detectar las
siguientes fallas:

- Defectos en los engranajes
- Defectos en los rodamientos
- Desalineamientos
- Desbalances
- Ejes torcidos
- Excentricidad
- Fallas eléctricas
- Fuerzas hidráulicas o aerodinámicas
- Mala sujeción en las piezas
- Problemas en las correas de transmisión
- Problemas de lubricación
- Resonancia
- Rozamientos en el rotor

## Vibración

Se conoce como vibración, al movimiento periódico de un cuerpo o medio
elástico, alrededor de un punto de equilibrio. En general podemos decir que una
vibración es un caso especifico de una oscilación, cuando esta es de origen
mecánico.


## Adquisición de datos

Para realizar cualquier tipo de análisis, primero se deben adquirir datos, y
por regla general mientras mas datos se tengan y mas precisas sean las
mediciones, mejores serán los estudios que se pueden realizar.

La toma de datos comienza con el sensor, que es el dispositivo que transforma
la unidad física de interés, en una señal que pueda ser procesada con mayor
facilidad. En el caso de las vibraciones, los sensores mas usados son los
acelerometros.  Esto se debe principalmente a que tienen mayor ancho de banda
que los sensores de posición y los de velocidad, lo que les permite detectar
vibraciones de mayor frecuencia. Adicionalmente, las vibraciones en los
rodamientos por naturaleza son de alta frecuencia, y debido a que estos son
componentes críticos en los motores eléctricos; hace casi exclusivo el uso de
acelerometros en las mediciones de vibración en motores eléctricos. Sin
embargo, en casos mas especializados, como podría ser el análisis de vibración
de maquinaria de larga envergadura son también usados los otros tipos de
sensores.

## Acelerometros

Se conoce como acelerometro a los dispositivos capaces de medir aceleración. Su
funcionamiento proviene de la segunda ley de Newton, que dice que fuerza
ejercida sobre un cuerpo es proporcional a su masa y a su aceleración. Los
acelerometros por lo general cuentan con una masa de prueba (también conocida
como masa sísmica), alguna especie de resorte y un marco de soporte, que a su
vez puede funcionar como amortiguador. Debido a esto, los acelerometros se
pueden modelar como un sistema lineal de segundo orden, por lo que su respuesta
en frecuencia posee un pico de resonancia.

## Tipos de acelerometros

### Acelerometros Capacitivos:

Los acelerometros capacitivos son uno de los modelos mas sencillos de medir
aceleración. Cuando una masa sísmica experimenta una fuerza, se desplaza a una
aceleración proporcional a la fuerza aplicada. Si a su vez a la masa se le
agrega unos resortes unidos a una carcasa, los resortes ejercerán una fuerza
proporcional al desplazamiento de la masa. Estos efectos juntos al
amortiguamiento producen un sistema lineal de segundo orden, el cual podemos
ver como un sistema que al aplicarse una fuerza de entrada produce un
desplazamiento de salida. Finalmente, si conectamos un sensor de
desplazamiento, podemos medir la aceleración. El sensor de desplazamiento mas
popular para este tipo de medidores es el capacitivo.

En su mayoría los acelerometros capacitivos vienen como dispositivos
microelectromecanicos (MEMS por sus siglas en ingles), que son dispositivos
fabricados con técnicas similares a la de la fabricación de circuitos
integrados, pero a su vez poseen componentes mecánicos microscópicos. Son los
acelerometros mas populares en aplicaciones no industriales, pero en la
industria son preferidos los acelerometros pizoresistivos y los pizoelectricos.
Aunque en aplicaciones de bajo consumo, bajo coste o cuando las frecuencias con
las que se trabajan no son tan altas, pueden ser usados en aplicaciones
industriales, ya que poseen múltiples ventajas como que no requieren de una
unidad de adecuación de la señal y pueden comunicarse directamente con un
microcontrolador; son bastante económicos, ya que pueden ser producidos en
masa con alta facilidad y son bastante compactos.

### Acelerometros piezoresistivos:

Son después de los acelerometros pizoelectricos, los mas usados a nivel
industrial. Están constituidos por una o varias galgas extensiométricas, una
masa de prueba y unos resortes de soporte. La galga sujeta a la masa de
sísmica, y al esta recibir una fuerza produce un desplazamiento proporcional a
la fuerza aplicada, lo que deforma a su vez la galga extensiométrica y
finalmente esto se traduce como un cambio de resistencia del sensor. La ventaja
de los acelerometros piezoresistivos es que pueden medir valores DC lo que los
hace útil en el estudio de impactos, sin embargo, son también usados en el
analisis de vibración en el rango de mediana frecuencia.

### Acelerometros piezoelectricos:

Son el acelerometro mas usado en aplicaciones industriales y poseen alto rango
dinámico, bajos niveles de ruido, alta linealidad, alto ancho de banda y al no
poseer partes móviles poseen poco desgaste. Su construcción es bastante
sencilla, se tiene disco de un cristal pizoelectrico unido por dos terminales
circulares, de forma similar a la de un condensador, y justo encima se tiene
una masa de prueba. Al experimentar una fuerza el cristal se deforma lo que
produce una diferencia de carga y un voltaje proporcional a la fuerza aplicada.
Como la aceleración de la masa de prueba es también proporcional a la fuerza
aplicada, la aceleración del acelerometro sera entonces directamente
proporcional al voltaje y la carga producida en el cristal.


# Procesamiento de señales

Una vez recolectado los datos el siguiente paso será análisis de los mismos.
Existen una gran variedad de técnicas, y la elección de una dependerá en mayor
medida de lo que se desea diagnosticar. Los análisis se clasificaran en dos
categorías principales: análisis de frecuencia y análisis en el dominio del
tiempo.

El análisis en frecuencia es el mas popular de los dos, esto se debe a
que la mayoría de las fallas poseen frecuencias características, y como el
análisis de frecuencia permite separar las frecuencias, esto facilita su
detección. Sin embargo, cuando las frecuencias son bajas o la frecuencia que se
quiere detectar se encuentra cerca de otro frecuencia, es muy difícil
identificar la señal en el dominio de la frecuencia. En estos casos es mejor
usar un análisis en el dominio del tiempo, ya que son mucho mas sencillas de
detectar las fallas.



# Quizas se deba agregar

Coherencia de señales ->

Otro tipo de análisis es el de coherencia de dos señales, cuando dos señales
son coherentes es bastante probable que estén correlacionadas por lo tanto se
puede estudiar una conociendo la otra.

Modulación ->

En el caso de rodamientos una técnica altamente usada es la de de demodulación
o la de envolvente, donde primero se necesita usar un filtro pasa altas para
luego desmodular la señal


# Referencias

- https://simple.wikipedia.org/wiki/Sensor
- https://en.wikipedia.org/wiki/Vibration
- https://en.wikipedia.org/wiki/Oscillation
- https://realpars.com/vibration-sensor/
- https://en.wikipedia.org/wiki/Microelectromechanical_systems
- https://www.machinedesign.com/mechanical-motion-systems/article/21837036/whats-the-difference-between-vibration-sensors

- Pizoelectric accelerometers, theory and aplication.
- Paresh Girdhar - Practical Machinery Vibration Analysis and Predictive Maintenance
- Jacob Fraden - Electronics Handbook of Modern Sensors Physics Designs and Applications-Springer (2003)
