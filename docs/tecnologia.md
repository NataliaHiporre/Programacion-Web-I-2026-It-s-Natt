## Módulo: Introducción a la Electricidad y Leyes Fundamentales

### Capítulo 1: Ley de Ohm y Potencia Eléctrica

#### 1.1 Ley de Ohm

La intensidad de corriente que circula por un circuito es directamente proporcional a la tensión aplicada e inversamente proporcional a su resistencia.

> 📷 **[Espacio para Imagen 1: Triángulo de la Ley de Ohm V / R | I]**

- **I (Intensidad de corriente):** Es el flujo de electrones que circula por el conductor. Se mide en **Amperes (A)**.
  $$I = \frac{V}{R}$$
  - _Conversión técnica:_ Para pasar de A a mA se multiplica por 1000 (1 A = 1000 mA); para pasar de mA a A se divide por 1000.
- **V (Tensión o Voltaje):** Es la fuerza que impulsa a los electrones (la corriente) a través del circuito. Se mide en **Volts (V)**.
  $$V = R \cdot I$$
- **R (Resistencia):** Es la dificultad u oposición que presenta el material al paso de la corriente eléctrica. Se mide en **Ohms (Ω)**.
  $$R = \frac{V}{I}$$

---

#### 1.2 Analogía Hidráulica

Para entender el comportamiento, imagina un circuito como una manguera:

- La **tensión** es la presión del agua.
- La **intensidad** es el caudal que circula.
- La **resistencia** es lo angosta o estrangulada que está la manguera.

**Conclusión:** A más presión (más voltaje) habrá más caudal (más corriente); pero si la manguera se estrangula (más resistencia), pasará menos caudal (menos corriente).

---

#### 1.3 Potencia Eléctrica en Corriente Continua (CC)

Es la cantidad de energía transferida por una fuente a un circuito por unidad de tiempo. Por el principio de conservación de la energía, esta no se pierde, sino que se transforma en otra manifestación energética.

- **P (Potencia):** Es la cantidad de energía transferida o transformada. Se mide en **Watts (W)**.
  $$P = V \cdot I$$
- **V (Tensión o Voltaje):** Es la tensión aplicada al circuito. Se mide en **Volts (V)**.
  $$V = \frac{P}{I}$$
- **I (Intensidad de corriente):** Es la corriente que circula por el circuito. Se mide en **Amperes (A)**.
  $$I = \frac{P}{V}$$

##### Explicación del Desfase (Uso de la Fórmula)

La fórmula general real de la potencia incluye el desfasaje entre la tensión y la corriente:
$$P = V \cdot I \cdot \cos(\varphi)$$

Sin embargo, en **Corriente Continua (CC)** ese desfasaje es de 0°. Como $\cos(0^\circ) = 1$, la fórmula se simplifica directamente a:
$$P = V \cdot I$$

---

### Capítulo 2: Concepto y Análisis de Circuitos

#### 2.1 El Circuito Eléctrico

Es un conjunto de elementos o componentes interconectados (como resistencias, diodos, capacitores, bobinas o pilas) de tal forma que debe haber, al menos, una **trayectoria cerrada**.

- **Condición de funcionamiento:** El conductor debe formar un camino cerrado para que los electrones puedan fluir de un polo a otro. Si se desconecta un extremo, la corriente se interrumpe a cero.
- **Peligro de cortocircuito:** No se debe conectar un alambre directo entre los terminales de una fuente. Como la resistencia tiende a cero, se generará una corriente destructiva que calentará el cable y la fuente, corriendo el riesgo de dañarla.

#### 2.2 Nodos

Se llama nodo al punto de interconexión donde se unen dos o más componentes.

> 📷 **[Espacio para Imagen 2: Esquema de Nodos simplificados - Nodo 1 y Nodo 2]**

- **Regla de análisis:** Si dos puntos están unidos por conductores perfectos (cables limpios sin ningún componente en el medio), representan **un solo y único punto** en el circuito. Aunque el dibujo cambie la forma de la conexión gráfica, su potencial eléctrico es el mismo.

---

#### 2.3 Circuitos con Resistencias en Serie

Las resistencias están conectadas una a continuación de la otra, de tal forma que la corriente que atraviesa la primera será exactamente la misma que atraviesa las siguientes.

> 📷 **[Espacio para Imagen 3: Circuito Serie con R1 y R2]**

- **Corriente total ($I_t$):** Es igual en todos los componentes del circuito.
  $$I_t = I_1 = I_2 = \dots = I_n$$
- **Tensión total ($V_t$):** La tensión de la fuente se reparte (cae) entre todas las resistencias.
  $$V_t = V_1 + V_2 + \dots + V_n$$
- **Resistencia total ($R_t$):** Es la suma directa de los valores de todas las resistencias.
  $$R_t = R_1 + R_2 + \dots + R_n$$

---

#### 2.4 Circuitos con Resistencias en Paralelo

Las resistencias están conectadas de tal forma que sus terminales de entrada están unidos entre sí, y sus terminales de salida también, quedando conectadas a los mismos dos nodos.

> 📷 **[Espacio para Imagen 4: Circuito Paralelo con R1 y R2]**

- **Corriente total ($I_t$):** La corriente se divide entre todos los caminos en paralelo disponibles.
  $$I_t = I_1 + I_2 + \dots + I_n$$
- **Tensión total ($V_t$):** El voltaje es exactamente el mismo en cada una de las resistencias.
  $$V_t = V_1 = V_2 = \dots = V_n$$
- **Resistencia total ($R_t$):** La inversa de la resistencia total es igual a la suma de las inversas de las resistencias.
  $$R_t = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2} + \dots + \frac{1}{R_n}}$$

---

### Capítulo 3: Leyes Fundamentales de Circuitos (Kirchhoff)

#### 3.1 Ley de Kirchhoff de Corrientes (Ley de Nodos)

La sumatoria de las corrientes eléctricas que entran y salen de un nodo es igual a cero en todo instante de tiempo (asignando signo positivo a las que entran y negativo a las que salen).

$$\sum_{k=1}^{n} I_k = 0 \Longleftrightarrow \sum I_{\text{entrada}} = \sum I_{\text{salida}}$$

> 📷 **[Espacio para Imagen 5: Distribución de corrientes en un Nodo central]**

#### 3.2 Ley de Kirchhoff de Tensiones (Ley de Mallas)

La sumatoria de las tensiones a lo largo de un circuito cerrado (malla), dando signo positivo (+) a las subidas de tensión y signo negativo (-) a las caídas de potencial, es igual a cero en todo instante de tiempo.

$$\sum_{k=1}^{n} V_k = 0 \Longleftrightarrow \sum V_{\text{subidas}} = \sum V_{\text{caídas}}$$
$$V_{\text{total}} = V_1 + V_2 + \dots + V_n$$

> 📷 **[Espacio para Imagen 6: Circuito cerrado con fuentes y caídas de tensión de 15V, 5V, 3V, 6V, 1V]**

---

### Capítulo 4: Componentes Pasivos en Corriente Continua

#### 4.1 Condensador o Capacitor ($C$)

Están compuestos por dos placas metálicas enfrentadas separadas por un aislante llamado dieléctrico (mica, aire, cerámica, etc.). Tienen la capacidad de almacenar cargas eléctricas. Su propiedad se llama **Capacidad** y se mide en **Faradios (F)**.

> 📷 **[Espacio para Imagen 7: Símbolo del Capacitor]**

##### Comportamiento en CC

Al conectar un capacitor a corriente continua, la tensión sobre él sube lentamente hasta alcanzar el valor máximo de la fuente, momento en el cual bloquea por completo el paso de la corriente.

> 📷 **[Espacio para Imagen 8: Gráfico de curva de carga de tensión Vc respecto al tiempo]**

- **Analogía hidráulica:** Es como un tanque de agua intercalado en la cañería. Al principio está vacío y el agua entra rápido. A medida que se llena, la presión interna sube hasta igualarse con la de la red; en ese punto, el tanque se llena y el agua deja de circular.

#### 4.2 Inductores o Bobinas ($L$)

Son elementos formados por un conductor arrollado sobre un núcleo. Tienen la característica de acumular energía en forma de campo magnético proporcional a la corriente que los atraviesa. Su valor se mide en **Henrios (H)**.

##### Comportamiento en CC

En el primer instante de conexión, la tensión crece bruscamente sobre el inductor debido a la fuerza contraelectromotriz (Fem) que genera para oponerse al cambio de corriente, y luego cae hasta tender a 0 Volts (comportándose como un cable directo o cortocircuito ideal).

> 📷 **[Espacio para Imagen 9: Gráfico de curva de tensión Vl respecto al tiempo]**

- **Analogía hidráulica:** Imagina una rueda de paletas muy pesada metida adentro de la tubería. Al principio, el agua choca y la rueda ofrece mucha resistencia para arrancar (pico de tensión). A medida que el agua la empuja, la rueda gira libremente a la misma velocidad del flujo y deja de oponer resistencia.

---

### Capítulo 5: Corriente Alterna y Filtros

#### 5.1 Fundamentos de Corriente Alterna (CA)

A diferencia de la corriente continua pura (valores constantes que no cambian de signo) o la pulsante (varía en magnitud pero mantiene el mismo signo), la **Corriente Alterna** varía su amplitud y cambia de signo de manera cíclica a lo largo del tiempo.

> 📷 **[Espacio para Imagen 10: Gráficos comparativos de continua pura, pulsante y alterna]**

En esta materia nos enfocamos en la **onda senoidal**, la cual surge de proyectar las variaciones de amplitud del círculo trigonométrico:

> 📷 **[Espacio para Imagen 11: Círculo trigonométrico y onda senoidal con radianes]**

##### Propiedades Fundamentales de la Onda

- **Ciclo:** Es el recorrido completo entre dos puntos equivalentes y consecutivos de la onda.
- **Período ($T$):** Es el tiempo que tarda la señal en realizar un ciclo completo. Se mide en **segundos (s)**.
- **Frecuencia ($f$):** Es la cantidad de ciclos completados por segundo. Se mide en **Hertz (Hz)**.

$$T = \frac{1}{f} \quad \text{y} \quad f = \frac{1}{T}$$

> 📷 **[Espacio para Imagen 12: Gráfico del período T en una onda senoidal]**

---

#### 5.2 Comportamiento de Componentes en Alterna

- **Reactancia Capacitiva ($X_c$):** Es la oposición que presenta un capacitor al paso de la corriente alterna. Se mide en Ohms (Ω) y su naturaleza vectorial se ubica a -90° respecto al eje real.
  $$|X_c| = \frac{1}{2\pi \cdot f \cdot C}$$
- **Reactancia Inductiva ($X_l$):** Es la oposición que presenta una bobina al paso de la corriente alterna. Se mide en Ohms (Ω) y su vector se ubica a +90° respecto al eje real.
  $$|X_l| = 2\pi \cdot f \cdot L$$

> 📷 **[Espacio para Imagen 13: Diagramas vectoriales de R, Xc y Xl sobre los ejes coordenados]**

##### Desfasaje según el componente

1. **Circuito puramente resistivo:** La tensión y la corriente están en fase (0° de separación).
2. **Circuito puramente inductivo:** La tensión adelanta a la corriente en 90°.
3. **Circuito puramente capacitivo:** La tensión atrasa a la corriente en 90°.

> 📷 **[Espacio para Imagen 14: Gráficos de ondas desfasadas para circuitos R, L y C]**

---

### Capítulo 6: Circuitos Complejos y Resonancia

#### 6.1 Circuito RLC Serie e Impedancia ($Z$)

La **Impedancia (Z)** es la oposición total que un circuito RLC serie presenta al paso de la corriente alterna. Como las reactancias y la resistencia tienen diferentes ángulos, su suma se realiza de forma estrictamente **vectorial**.

- **Pulsación ($\omega$):** Simplifica las expresiones de las reactancias mediante la relación $\omega = 2\pi f$ (medida en rad/s).
  $$|X_c| = \frac{1}{\omega \cdot C} \quad \text{y} \quad |X_l| = \omega \cdot L$$

##### Análisis Analítico (Fórmulas)

- **Módulo de la Impedancia:**
  $$|Z| = \sqrt{R^2 + (X_l - X_c)^2}$$
  $$|Z| = \sqrt{R^2 + \left(2\pi f L - \frac{1}{2\pi f C}\right)^2}$$
- **Ángulo de desfasaje ($\rho$):**
  $$\tan(\rho) = \frac{X_l - X_c}{R} \implies \rho = \arctan\left(\frac{X_l - X_c}{R}\right)$$

> 📷 **[Espacio para Imagen 15: Suma geométrica de vectores para hallar Z]**

#### 6.2 Frecuencia de Resonancia ($f_0$)

Cuando la frecuencia del circuito hace que los efectos de la bobina y del capacitor se igualen ($X_l = X_c$), ambas reactancias se anulan por completo. En ese instante exacto, la impedancia cae a su valor mínimo ($Z = R$), lo que provoca que **la corriente circulante por el circuito sea máxima**.

$$f_0 = \frac{1}{2\pi\sqrt{L \cdot C}}$$

---

### Capítulo 7: Aplicaciones Técnicas - Filtros Pasivos

Los filtros utilizan combinaciones de componentes pasivos para permitir el paso de frecuencias específicas y bloquear otras. Consideramos el transmisor como la señal de entrada ($Tx$) y el receptor como la carga ($Rx$).

#### 7.1 Filtro Pasa Altos

Permite el paso de las frecuencias altas y bloquea las bajas. Se logra conectando un **capacitor en serie** entre el $Tx$ y el $Rx$.

> 📷 **[Espacio para Imagen 16: Esquema de circuito Pasa Altos con capacitor en serie]**

- **Explicación:** Si la frecuencia ($f$) sube, la reactancia $X_c$ baja, permitiendo mayor paso de corriente hacia la carga. Si la frecuencia baja hacia cero (CC), $X_c$ tiende a infinito, actuando como un circuito abierto.

> 📷 **[Espacio para Imagen 17: Curva de respuesta en potencia del filtro Pasa Altos y frecuencia de corte inferior Fci]**

#### 7.2 Filtro Pasa Bajos

Permite el paso de las frecuencias bajas y atenúa las altas. Se logra conectando un **inductor en serie** entre el $Tx$ y el $Rx$.

> 📷 **[Espacio para Imagen 18: Esquema de circuito Pasa Bajos con inductor en serie]**

- **Explicación:** A bajas frecuencias, la reactancia $X_l$ es casi nula, comportándose como un cortocircuito que no opone resistencia. A altas frecuencias, $X_l$ crece proporcionalmente hasta bloquear el paso de la señal.

> 📷 **[Espacio para Imagen 19: Curva de respuesta en potencia del filtro Pasa Bajos y frecuencia de corte superior Fcs]**

#### 7.3 Filtro Pasa Banda (Circuito RLC Serie)

Un circuito RLC en serie permite el paso de una banda específica de frecuencias que se encuentra alrededor de su frecuencia de resonancia ($f_0$), donde la impedancia es mínima.

> 📷 **[Espacio para Imagen 20: Esquema de circuito Pasa Banda RLC Serie]**

- **Ancho de Banda (AB):** Es el rango de frecuencias comprendido entre la frecuencia de corte inferior ($f_{ci}$) y la de corte superior ($f_{cs}$) donde se concentra la mayor potencia de la señal (delimitado técnicamente por la caída de -3 dB, que equivale a la mitad de la potencia máxima).

$$AB = f_{cs} - f_{ci}$$

> 📷 **[Espacio para Imagen 21: Campana de respuesta del filtro Pasa Banda con fci, fo, fcs y ancho de banda]**
