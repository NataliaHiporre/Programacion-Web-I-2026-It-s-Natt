## Módulo: Introducción a la Electricidad y Leyes Fundamentales

### Capítulo 1: Ley de Ohm y Potencia Eléctrica

#### 1.1 Ley de Ohm

La intensidad de corriente que circula por un circuito es directamente proporcional a la tensión aplicada e inversamente proporcional a su resistencia.

![Ley de Ohm](./img/Tec/1.png)

- **I (Intensidad de corriente):** Es el flujo de electrones que circula por el conductor. Se mide en **Amperes (A)**.
  $$I = \frac{V}{R}$$
  - _Conversión técnica:_ Para pasar de A a mA se multiplica por 1000 (1 A = 1000 mA); para pasar de mA a A se divide por 1000.
- **V (Tensión o Voltaje):** Es la fuerza que impulsa a los electrones (la corriente) a través del circuito. Se mide en **Volts (V)**.
  $$V = R \cdot I$$
- **R (Resistencia):** Es la dificultad u oposición que presenta el material al paso de la corriente eléctrica. Se mide en **Ohms (Ω)**.
  $$R = \frac{V}{I}$$

---

#### 1.2 Analogía Hidráulica

Para entender el comportamiento, imagina un circuito como una manguera: la tensión es la presión del agua, la intensidad es el caudal que circula y la resistencia es lo angosta que está la manguera.

**Conclusión:** Por ende, a más presión (más voltaje) habrá más caudal (más corriente); pero si la manguera se estrangula (más resistencia), pasará menos caudal (menos corriente).

---

#### 1.3 Potencia Eléctrica en Corriente Continua (CC)

Es la cantidad de energía transferida por una fuente a un circuito por unidad de tiempo. Por el principio de conservación de la energía, esta energía no se pierde, sino que se transforma en otra manifestación energética.

![Potencia Eléctrica](./img/Tec/2.png)

- **P (Potencia):** Es la cantidad de energía transferida o transformada. Se mide en **Watts (W)**.
  $$P = V \cdot I$$
- **V (Tensión o Voltaje):** Es la tensión aplicada al circuito. Se mide en **Volts (V)**.
  $$V = \frac{P}{I}$$
- **I (Intensidad de corriente):** Es la corriente que circula por el circuito. Se mide en **Amperes (A)**.
  $$I = \frac{P}{V}$$

##### Explicación del Desfase (Uso de la Fórmula)

La fórmula general real de la potencia incluye el desfasaje entre la tensión y la corriente, y es:
$$P = V \cdot I \cdot \cos(\varphi)$$

Sin embargo, en **Corriente Continua (CC)** ese desfasaje es de 0°. Como el coseno de 0 grados es igual a 1, la fórmula se simplifica directamente a:
$$P = V \cdot I$$

---

### Capítulo 2: Concepto y Análisis de Circuitos

#### 2.1 El Circuito Eléctrico

Es un conjunto de elementos o componentes interconectados (como resistencias, diodos, capacitores, bobinas o pilas) de tal forma que debe haber, al menos, una **trayectoria cerrada**.

- **Condición de funcionamiento:** El conductor debe formar una trayectoria cerrada para que los electrones puedan fluir. Si se conecta un cable a los dos terminales de una pila, la corriente fluye porque el camino está cerrado. Si sólo se conecta un extremo, no hay corriente porque los electrones no tienen hacia dónde ir.
- **Peligro de cortocircuito:** No se debe conectar un alambre directo entre los terminales de una fuente. Como la resistencia es muy baja, se generará una gran corriente que calentará el cable y la pila, corriendo el riesgo de dañar la fuente. Para aprovechar la corriente, siempre se deben incluir componentes que interactúen con ella.

#### 2.2 Nodos

Se llama nodo al punto de interconexión donde se unen dos o más componentes.

- **Regla de análisis para los Nodos:** Si dos puntos están unidos por conductores perfectos (cables limpios sin ningún componente en el medio), en teoría representan un solo y único punto en el circuito. Considerar que son dos nodos diferentes es un error común; aunque el dibujo cambie la forma de la conexión y los muestre separados, son en realidad un solo punto.

![Regla de análisis para los Nodos](./img/Tec/3.png)

---

#### 2.3 Circuitos con Resistencias en Serie

Las resistencias están conectadas una a continuación de la otra en el circuito eléctrico, de tal forma que la corriente que atraviesa la primera de ellas será la misma que atraviesa las siguientes.

![Circuitos con Resistencias en Serie](./img/Tec/4.png)

- **Corriente total ($I_t$):** La corriente total es igual en todos los componentes del circuito.
  $$I_t = I_1 = I_2 = \dots = I_n$$
- **Tensión total ($V_t$):** La tensión de la fuente, voltaje total, se reparte entre todas las resistencias.
  $$V_t = V_1 + V_2 + \dots + V_n$$
- **Resistencia total ($R_t$):** Es la suma directa de los valores de todas las resistencias.
  $$R_t = R_1 + R_2 + \dots + R_n$$

---

#### 2.4 Circuitos con Resistencias en Paralelo

Las resistencias están conectadas de tal forma que sus terminales de entrada están unidos entre sí, y sus terminales de salida también, quedando todas conectadas directamente a los mismos dos nodos del circuito.

![Circuitos con Resistencias en Paralelo](./img/Tec/5.png)

- **Corriente total ($I_t$):** La corriente total se divide entre todos los caminos en paralelo.
  $$I_t = I_1 + I_2 + \dots + I_n$$
- **Tensión total ($V_t$):** El voltaje total es exactamente el mismo en cada una de las resistencias, ya que todas comparten los mismos nodos.
  $$V_t = V_1 = V_2 = \dots = V_n$$
- **Resistencia total ($R_t$):** La inversa de la resistencia total es igual a la suma de las inversas de cada una de las resistencias.
  $$R_t = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}}$$

---

### Capítulo 3: Leyes Fundamentales de Circuitos (Kirchhoff)

#### 3.1 Ley de Kirchhoff de Corrientes (Ley de Nodos)

La sumatoria de las corrientes eléctricas que entran y salen de un nodo, dando signo positivo (+) a las que entran y signo negativo (-) a las que salen, es igual a 0 en todo instante de tiempo.

$$\sum_{k=1}^{n} I_k = 0 \Longleftrightarrow \sum I_{\text{entrada}} = \sum I_{\text{salida}}$$

![Ley de Kirchhoff de Corrientes](./img/Tec/6.png)

#### 3.2 Ley de Kirchhoff de Tensiones (Ley de Mallas)

La sumatoria de las tensiones a lo largo de un circuito cerrado (malla), dando signo positivo (+) a las subidas de tensión y signo negativo (-) a las caídas de potencial, es igual a 0 en todo instante de tiempo. Esto equivale a decir que la suma de las caídas de potencial es igual a la tensión aplicada al mismo.

$$\sum_{k=1}^{n} V_k = 0 \Longleftrightarrow \sum V_{\text{subidas}} = \sum V_{\text{caídas}}$$
$$V_{\text{total}} = V_1 + V_2 + \dots + V_n$$

![Ley de Kirchhoff de Tensiones](./img/Tec/7.png)

---

### Capítulo 4: Componentes Pasivos en Corriente Continua

#### 4.1 Condensador o Capacitor

Son componentes que tienen ciertas particularidades especiales. Están compuestos por 2 placas metálicas enfrentadas separadas por un aislante (puede ser mica, el aire, cerámica, etc.) llamado dieléctrico. Tienen la capacidad de almacenar cargas cuando están conectados en un circuito eléctrico de corriente continua. Se lo identifica con la letra C, su característica de almacenar cargas se llama Capacidad y se mide en Faradios (F).

![Condensador o Capacitor](./img/Tec/8.png)

##### Comportamiento de un condensador en corriente continua

Al conectar el circuito, la tensión sobre el condensador sube lentamente hasta alcanzar un valor máximo.

![Comportamiento de un condensador en CC - Gráfico 1](./img/Tec/9.png)
![Comportamiento de un condensador en CC - Gráfico 2](./img/Tec/10.png)

- **Analogía hidráulica:** Para entender el comportamiento, imaginate que un capacitor es como un tanque de agua intercalado en la cañería. Al principio, el tanque está vacío y el agua empieza a entrar llenándolo lentamente. A medida que el tanque se va llenando, la presión en el tanque sube despacito hasta que se iguala con la de la red; en ese momento, el tanque se llenó por completo y el agua deja de circular (bloquea el paso de la corriente).

#### 4.2 Inductores o Bobinas

También llamados comúnmente bobinas, son elementos eléctricos formados por un conductor arrollado sobre un núcleo no conductor.

![Inductores o Bobinas](./img/Tec/11.png)

Su comportamiento en corriente continua es acumular energía en forma de corriente eléctrica y una característica muy importante es generar un campo magnético a su alrededor proporcional a la corriente que lo atraviesa. Cuando se quiere quitar esa corriente el inductor responde generando una tensión igual pero de sentido inverso a la que producía la corriente que lo atravesaba. Esta tensión se denomina fuerza contraelectromotriz inducida (Fem). Su valor se mide en Henrios o Henry y se lo abrevia con (H) o (Hy).

##### Comportamiento de un inductor en corriente continua

Aquí se puede ver que en un primer instante la tensión crece bruscamente sobre el inductor y luego baja hasta tender a 0 Volts (en un conductor ideal).

![Comportamiento de un inductor en CC - Gráfico 1](./img/Tec/12.png)
![Comportamiento de un inductor en CC - Gráfico 2](./img/Tec/13.png)

- **Analogía hidráulica:** Para entender el inductor, imaginate una rueda de paletas pesada (un molino) metida adentro de la tubería. Al principio, cuando el agua empieza a correr, la rueda está totalmente quieta y ofrece muchísima resistencia para empezar a girar, provocando un gran frenazo de golpe (el pico brusco de tensión). A medida que el agua empuja, la rueda empieza a girar más y más rápido hasta que acompaña el flujo por completo; en ese punto, la rueda ya no frena nada el agua y gira libremente sin oponer resistencia (la tensión cae a 0 Volts).

---

### Capítulo 5: Corriente Alterna y Filtros

#### 5.1 Fundamentos de Corriente Alterna

Una tensión o corriente continua es aquella que no cambia de signo a través del tiempo. Se puede clasificar en continua pura o continua pulsante. Por otro lado, en la **Corriente Alterna** la amplitud cambia y se modifica a lo largo del tiempo.

![Fundamentos de Corriente Alterna](./img/Tec/14.png)

El gráfico de la figura 1 corresponde a esta definición pero los siguientes gráficos también.

![Corriente Alterna - Variación de gráficos 1](./img/Tec/15.png)
![Corriente Alterna - Variación de gráficos 2](./img/Tec/16.png)

En este caso el sentido de circulación de la corriente o la aplicación de la tensión cambia de signo.

![Corriente Alterna - Cambio de signo](./img/Tec/17.png)

El caso específico que estudiaremos en esta materia es el de la corriente alterna senoidal o sinusoidal el gráfico puede verse de la siguiente manera.

![Onda Senoidal Sinusoidal](./img/Tec/18.png)

y reflejada en un gráfico cartesiano es decir que cuando está hablando de la forma de la onda.

![Forma de onda en plano cartesiano](./img/Tec/19.png)

##### Propiedades de la Onda Senoidal

- **Ciclo:** Es el recorrido entre dos puntos iguales de la onda.
- **Período ($T$):** Es el tiempo que se tarda en realizar un ciclo. Se mide en segundos (s).
- **Frecuencia ($f$):** Es la cantidad de ciclos que se realizan por segundo. Se mide en Hertz (Hz).

![Propiedades de la onda senoidal](./img/Tec/20.png)

##### Fórmulas de onda:

$$T = \frac{1}{f} \quad \text{y} \quad f = \frac{1}{T}$$

---

#### 5.2 Comportamiento de Componentes en Alterna

- **Reactancia Capacitiva ($X_c$):** Es la oposición que presenta un condensador al paso de la corriente alterna. Se mide en Ohms (Ω).
  $$|X_c| = \frac{1}{2\pi \cdot f \cdot C}$$
- **Reactancia Inductiva ($X_l$):** Es la oposición que presenta un inductor al paso de la corriente alterna. Se mide en Ohms (Ω).
  $$|X_l| = 2\pi \cdot f \cdot L$$

##### Esquema Gráfico de Resistencias Vectoriales

###### Resistencia (R)

![Resistencia R](./img/Tec/21.png)

###### Reactancia Capacitiva ($X_c$)

![Reactancia Capacitiva Xc](./img/Tec/22.png)

###### Reactancia Inductiva ($X_l$)

![Reactancia Inductiva Xl](./img/Tec/23.png)

##### Desfasaje en Corriente Alterna

Es el ángulo de separación que se produce entre las ondas de tensión y de corriente al atravesar un componente.

![Símbolo del Generador](./img/Tec/24.png)

1. **Circuito totalmente resistivo:** La corriente sigue la misma forma de onda que la tensión, por lo que se dice que están en fase.

![Circuito Resistivo - Onda](./img/Tec/25.png)
![Circuito Resistivo - Esquema](./img/Tec/26.png)

2. **Circuito totalmente inductivo:** Las ondas se separan y se dice que la tensión adelanta a la corriente en 90°.

![Circuito Inductivo - Onda](./img/Tec/27.png)
![Circuito Inductivo - Esquema](./img/Tec/28.png)

3. **Circuito totalmente capacitivo:** Las ondas se separan y se dice que la tensión atrasa a la corriente en 90°.

![Circuito Capacitivo - Onda](./img/Tec/29.png)
![Circuito Capacitivo - Esquema](./img/Tec/30.png)

---

### Capítulo 6: Circuitos Complejos y Resonancia

#### 6.1 Circuito RLC Serie

- **Pulsación ($\omega$):** Relación matemática definida por $\omega = 2\pi f$ (rad/s).
- **Definición de Impedancia (Z):** Es la resistencia total que un circuito RLC serie presenta al paso de la corriente alterna. Se mide en Ohms (Ω). Al estar los componentes en serie, sus resistencias deben sumarse de forma vectorial.

![Definición de Impedancia Z](./img/Tec/31.png)

##### Suma Geométrica

Como $X_c$ y $X_l$ están sobre la misma recta de acción pero en sentidos opuestos, primero se restan directamente ($X_l - X_c$). El vector resultante de esa resta se combina a 90° con la resistencia R para formar la Impedancia (Z) y su ángulo de desfasaje ($\rho$).

![Suma Geométrica - Vector 1](./img/Tec/32.png)
![Suma Geométrica - Vector 2](./img/Tec/33.png)

##### Suma Analítica (Fórmulas)

- **Módulo de la Impedancia:**
  $$|Z| = \sqrt{R^2 + (X_l - X_c)^2} \implies |Z| = \sqrt{R^2 + \left(2\pi f L - \frac{1}{2\pi f C}\right)^2}$$
- **Ángulo de desfasaje:**
  $$\rho = \arctan\left(\frac{X_l - X_c}{R}\right)$$

#### 6.2 Frecuencia de Resonancia ($f_0$)

Cuando $X_l = X_c$, ambas reactancias se anulan por completo. En ese instante, la impedancia cae a su valor mínimo ($Z = R$) y la corriente es máxima.

$$f_0 = \frac{1}{2\pi\sqrt{L \cdot C}}$$

---

### Capítulo 7: Aplicaciones Técnicas - Filtros

Los filtros son circuitos compuestos por componentes pasivos que permiten el paso de ciertas frecuencias y bloquean otras. $Rx$ será el receptor y $Tx$ será el transmisor.

#### 7.1 Circuito Pasa Altos

Presentará una baja resistencia a las frecuencias altas en un circuito. Se logra conectando un condensador en serie entre el transmisor y el receptor.

![Circuito Pasa Altos](./img/Tec/34.png)

Recordemos la fórmula de $X_c$:
$$X_c = \frac{1}{2\pi f C}$$

Por lo contrario si la frecuencia F baja la reactancia sube y F tiende a cero Xc tiende al infinito lo que significa que se comporta como un circuito abierto No dejando pasar la señal.

![Circuito Pasa Altos - Bloqueo](./img/Tec/35.png)

#### 7.2 Circuito Pasa Bajos

Presentará una baja resistencia a las frecuencias bajas en un circuito. Se logra conectando un inductor en serie entre el transmisor y el receptor.

![Circuito Pasa Bajos](./img/Tec/36.png)

Recordamos la fórmula de $X_l$:
$$X_l = 2\pi f L$$

![Circuito Pasa Bajos - Respuesta](./img/Tec/37.png)

El gráfico muestra la distribución de la potencia de la señal que recibe el receptor a medida que la frecuencia aumenta cayendo la potencia cuando se supera la frecuencia de corte.

#### 7.3 Circuito Pasa Banda

Un circuito RLC serie funciona como un circuito **PASA BANDA**. Esto significa que habrá una banda pasante que tendrá un conjunto de frecuencias que tendrán menor Impedancia Z, o sea que tendrá menor resistencia al paso de la señal.

![Circuito Pasa Banda](./img/Tec/38.png)

Esa frecuencia será la frecuencia de resonancia, la central, y a sus lados una frecuencia de corte inferior $f_{ci}$ y una de corte superior $f_{cs}$. Fuera de esos límites se considera que las otras frecuencias están bloqueadas. Al conjunto de frecuencias entre la $f_{ci}$ y la $f_{cs}$ se la llama **ancho de banda (AB)**.

La línea que marca -3 _ D _ B es la única línea que indica que la señal está a mitad de la pendiente.

![Ancho de banda - Puntos de potencia media](./img/Tec/39.png)

##### Fórmulas de Cierre:

$$|Z| = \sqrt{R^2 + \left(2\pi f L - \frac{1}{2\pi f C}\right)^2}$$
$$f_0 = \frac{1}{2\pi\sqrt{L \cdot C}}$$
