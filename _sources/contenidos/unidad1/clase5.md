# Análisis del movimiento de un cuerpo rígido en rotación pura, en torno a un punto fijo ${\text{0}}$

> + El movimiento se describe por la ecuación de `Momento de la Fuerza:`.
> + Si se recuerda, para el caso de un `Sistema de N Partículas`, la ecuación de momento de la fuerza en torno a un punto fijo ${\text{0}}$:

$$
\begin{align*}
{\bf{M}}_{\text{0}}&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times {\bf{F}}_{i}
\end{align*}
$$

> + Ahora, para el sistema `cuerpo rígido`, la ecuación de Momento de la Fuerza o Torque, resultante alrededor del punto fijo ${\text{0}}$ será: 

$$
\begin{align*}
{\bf{M}}_{\text{0}}&=\int_{{\text{cuerpo}}}^{}{\bf{r}}\times \text{d}{\bf{{\text{F}}}}
\label{eq48}\tag{48}
\end{align*}
$$

> + También, si recordamos, vimos que para el mismo `Sistema de N Partículas`, el momentum angular del cuerpo en torno al punto fijo ${\text{0}}$ es: 

$$
\begin{align*}
{\bf{H}}_{\text{0}}&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times m_{i}{\bf{\dot{r}}}_{i}
\end{align*}
$$

> + Esta vez, en el caso de un sistema de cuerpo rígido:

$$
\begin{align*}
{\bf{H}}_{\text{0}}&=\int_{{\text{cuerpo}}}^{}{\bf{r}}\times {\bf{{\text{v}}}}\, \text{dm}
\label{eq49}\tag{49}
\end{align*}
$$

> + Pero, en el caso de `rotación pura en un plano`, anteriormente ya vimos que la velocidad tiene solamente una componente en dirección angular $\hat{\theta}$:

$$
\begin{align*}
{\bf{{\text{v}}}}&=r\,\dot{\theta}\,\hat{\theta}=r\,\omega\,\hat{\theta}
\end{align*}
$$

> + Reemplazando:

$$
\begin{align*}
{\bf{H}}_{\text{0}}&=\int_{{\text{cuerpo}}}^{}r\,\hat{r}\,\times\,r\,\omega\,\hat{\theta}\,\,\text{dm}= \Bigg(\int_{{\text{cuerpo}}}^{} r^{2}\,\text{dm} \Bigg)\,\omega\, \hat{k}\,=\,{\text{I}}_{\text{0}}\,\omega\, \hat{k}
\end{align*}
$$

+ >> donde:

$$
\begin{align*}
{\text{I}}_{\text{0}}&=\int_{{\text{cuerpo}}}^{} r^{2}\,\text{dm}
\end{align*}
$$

+ >> Se llama el `Momento de Inercia del Cuerpo Rígido` en torno al punto fijo ${\text{0}}.$ Por lo tanto, para movimiento planar, el momentum angular solamente tiene una componente: 

$$
\begin{align*}
{\bf{H}}_{\text{0}}&={\text{I}}_{\text{0}}\,\omega\, \hat{k}
\end{align*}
$$

> + Si se deriva con respecto al tiempo:

$$
\begin{align*}
{\bf{\dot{H}}}_{\text{0}}&={\text{I}}_{\text{0}}\,{\dot{\omega}}\, \hat{k}={\text{I}}_{\text{0}}\,{\alpha}\, \hat{k}
\end{align*}
$$

+ >> con $\alpha$ la **aceleración angular del cuerpo**. Pero, dado que se cumple la relación:

$$
\begin{align*}
{\bf{\dot{H}}}_{\text{0}}&={\bf{M}}_{\text{0}}
\end{align*}
$$

+ >> entonces, el momento de la fuerza será:

$$
\begin{align*}
{\bf{M}}_{\text{0}}&={\text{I}}_{\text{0}}\,{\alpha}\, \hat{k}
\end{align*}
$$

```{note}
Como ejercicio, vamos a analizar el movimiento de un péndulo compuesto.
```

+ > Un `Cuerpo Rígido` suspendido desde un punto distinto al centro de masa y libre de oscilar, se conoce como `Péndulo Compuesto`. 

+ > Vamos a suponer que tenemos el siguiente péndulo compuesto, consistente de una barra uniforme de masa total ${\text{m}}$ que cuelga en un punto ${\text{0}}$ a una distancia $\frac{{\text{L}}}{6}$ del centro de masa ${\text{C}}$. 
+ > Si el péndulo se libera desde el reposo, en la posición horizontal, se nos pide determinar la aceleración angular $\alpha$ del péndulo inmediatamente después de liberarse.

+ > ![Figura Señal2](compuesto.png)

```{note}
Desarrollo: 
```

> + Aquí, se aplica la relación: $\text{M}_{\text{0}}={\text{I}}_{\text{0}}\,{\alpha}$. Para obtener $\text{M}_{\text{0}}$ se deduce de la siguiente figura, que: 

+ > ![Figura Señal2](convencion2.png)

$$
\begin{align*}
\text{M}_{\text{0}}&=-\,{\text{mg}}\,\frac{\text{L}}{6}
\end{align*}
$$

> + Luego, se calcula el momento de inercia de la barra:

$$
\begin{align*}
{\text{I}}_{\text{0}}&=\int_{{\text{cuerpo}}}^{} x^{2}\,\text{dm}
\end{align*}
$$

+ > donde

$$
\begin{align*}
\text{dm}&=\rho\, \text{dx}=\frac{m}{L}\, \text{dx}
\end{align*}
$$

> + Por lo que se obtiene:

$$
\begin{align*}
{\text{I}}_{\text{0}}&=\frac{\text{m}}{L}\,\int_{-\frac{L}{3}}^{\frac{2L}{3}} x^{2}\,\text{dx}\\
&= \frac{\text{m}\,\text{L}^{2}}{9}
\end{align*}
$$

> + Por lo tanto, la aceleración angular $\alpha$ está dado por:

$$
\begin{align*}
\alpha&=\frac{\text{M}_{\text{0}}}{{\text{I}}_{\text{0}}}=-\frac{3\,{\text{g}}}{2\,{\text{L}}}
\end{align*}
$$

> + El signo menos indica que la aceleración angular sigue el sentido de las manecillas del reloj, esto es, va en el sentido contrario al señalado en la figura original.


```{note}
Problema propuesto para desarrollar en equipos: 
```


<!---
+ > `Cuerpo Rígido:` Se caracteriza porque tiene una masa que se distribuye de manera continua a lo largo del cuerpo.

+ > `Densidad de Masa:` Se define $\rho(x,y,z)$ como una función de densidad de masa que representa una masa por unidad de volumen.

+ > `Elemento Diferencial de Masa:` En el caso de un cuerpo rígido, vamos a reemplazar $m_{i}$ por: ${dm}\,(x,y,z)$.

+ > `Traslación:` Por analogía con un sistema de partículas:

$$
\begin{align*}
{\bf{F}}&=\,\sum_{i=1}^{N}m_{i}\,{\bf{\ddot{r}}}_{i}\,=\sum_{i=1}^{N}m_{i}\,{\bf{a}}_{i}\quad\quad {\text{i=1,2,}}\ldots{\text{N}}
\end{align*}
$$

```{note}
Para un cuerpo rígido, la fuerza resultante ${\bf{F}}(t)$ será igual a:
```

$$
\begin{align*}
{\bf{F}}(t)&=\,\int_{{\text{cuerpo}}}^{}{\bf{a}}(x,y,z,t)\,{dm}\,(x,y,z)
\label{eq39}\tag{39}
\end{align*}
$$

+ > Con ${\bf{a}}(x,y,z,t)$ el vector de aceleración en un punto sobre el cuerpo rígido y ${dm}\,(x,y,z)=\rho(x,y,z)\,dV$, siendo $V$ un elemento diferencial de volumen. 

```{note}
En `traslación pura`, se cumple que para todos los puntos del sistema de cuerpo rígido, la aceleración es la misma, es decir, ${\bf{a}}(x,y,z,t)={\bf{a}}(t)$. Por lo que la ecuación de movimiento del sistema quedará:
```

$$
\begin{align*}
{\bf{F}}(t)&=\,{\bf{a}}(t)\,\int_{{\text{cuerpo}}}^{}{dm}\,(x,y,z)
\label{eq40}\tag{40}
\end{align*}
$$

+ > Además, la masa total del sistema de cuerpo rígido es:

$$
\begin{align*}
\int_{{\text{cuerpo}}}^{}{dm}\,(x,y,z)&=m
\label{eq41}\tag{41}
\end{align*}
$$

+ > Así, la ecuación diferencial de movimiento queda expresada como:

$$
\begin{align*}
{\bf{F}}(t)&=\,m\,{\bf{a}}(t)
\label{eq42}\tag{42}
\end{align*}
$$

```{note}
Como ejercicio, obtener las ecuaciones de movimiento para el siguiente sistema de cuerpo rígido en traslación horizontal.
```
+ > ![Figura Señal2](ej1.png)

Las reacciones horizontales en los puntos de contacto $A$ y $B$, como se muestra en el dibujo, son proporcionales a las reacciones verticales en esos puntos, siendo la constante de proporcionalidad es el coeficiente de fricción $\mu$.

+ > Diagrama de cuerpo libre:
+ > ![Figura Señal2](ej2.png)

+ > Usar los valores: $\beta = 30^{\text{o}}$; $\mu = 0.5$; $\text{H}=0.6\,{\text{L}}$; y $\text{D}=0.1\,{\text{L}}$, y determinar la magnitud de la fuerza, $\text{F}$, como una fracción del peso, $\text{m}{\text{g}}$, cuando el cuerpo está a punto de volcar (pero no se vuelca!), al igual que la aceleración del cuerpo como una fracción de $\text{g}$. 

+ > Al desarrollar el ejercicio, se observa lo siguiente:

* El problema es bidimensional, todo ocurre en el plano-xy.
    + Por lo cual, las ecuaciones de fuerza tienen solamente dos componentes escalares: $\text{F}_{x}=\text{m}\text{a}_{x}$ y $\text{F}_{y}=\text{m}\text{a}_{y}$
* El cuerpo en traslación horizontal solamente tiene aceleración en dirección $\text{x}$.
* En el instante de casi volcar, en el punto de contacto $\text{A}$, la reacción normal, $\text{N}_{\text{A}}=0$.

* En el DCL, se representan las siguientes fuerzas:   
    + La fuerza aplicada en la esquina superior izquierda ${\text{F}}$.
    + El peso que apunta verticalmente hacia abajo y pasa por el centro de masa.
    + La fuerza normal $\text{N}_{\text{B}}$ en el punto de contacto $\text{B}$.
    + La fuerza de fricción ${\text{F}_{\text{B}}}$ en el punto de contacto $\text{B}$


<!---
+ > Nuestras `variables lineales` han sido:

> * Posición: ${\bf{\text{r}}}(t)$
> * Velocidad: ${\bf{\dot{r}}}(t)$
> * Aceleración: ${\bf{\ddot{r}}}(t)$

+ > Y nuestra variables `rotacionales` han sido:

* Desplazamiento angular:
    + $\theta (t)$
* Velocidad angular:
    + $\omega (t) = \dot{\theta} (t)$
* Aceleración angular:    
    + $\alpha (t) = \dot{\omega}(t) = \ddot{\theta}(t)$

+ > Para derivar las ecuaciones de movimiento de un sistema de $N$, se deben distinguir dos tipos de fuerzas que actúan sobre el sistema:

+ >> Las `Fuerzas Externas:` ${\bf{\text{F}}}_{i}$
+ >> Y las `Fuerzas Internas:` estas surgen por la interacción entre las partículas: ${\bf{f}}_{ij}$, que representa la fuerza ejercida por la masa $m_j$ sobre la masa $m_i$ ($i,j=1,2,\ldots, N; j\ne i$). 

+ > ![Figura Señal2](fext_int.png)

+ > La ecuación de movimiento para la partícula $m_i$, se obtiene usando la segunda Ley de Newton:

$$
\begin{align*}
{\bf{\text{F}}}_{i}+\sum_{j=1}^{N}{\bf{f}}_{ji}&=m_{i}\,{\bf{\ddot{r}}}_{i},\quad\quad {\text{i=1,2,}}\ldots{\text{N}} 
\label{eq26}\tag{26}
\end{align*}
$$

+ > Y la ecuación de movimiento ahora para el sistema total de N partículas, será:

$$
\begin{align*}
\sum_{i=1}^{N}{\bf{\text{F}}}_{i}+\sum_{i=1}^{N}\sum_{j=1}^{N}{\bf{f}}_{ji}&=\,\sum_{i=1}^{N}m_{i}\,{\bf{\ddot{r}}}_{i},\quad\quad {\text{i=1,2,}}\ldots{\text{N}}
\label{eq27}\tag{27}
\end{align*}
$$

+ > Sin embargo, por la Tercera Ley de Newton, las fuerzas internas se cancelan en pares: ${\bf{f}}_{ji}+{\bf{f}}_{ij} = {\bf{0}}$

+ > Si llamamos ahora ${\bf{F}}$ a la `fuerza resultante` debido a todas las fuerzas externas, entonces

$$
\begin{align*}
{\bf{F}}&=\sum_{i=1}^{N}{\bf{\text{F}}}_{ext^{i}} 
\label{eq28}\tag{28}
\end{align*}
$$

+ > La ecuación de movimiento para el sistema de $N$ partículas queda de la forma:

$$
\begin{align*}
{\bf{F}}&=\,\sum_{i=1}^{N}m_{i}\,{\bf{\ddot{r}}}_{i},\quad\quad {\text{i=1,2,}}\ldots{\text{N}}
\label{eq29}\tag{29}
\end{align*}
$$

+ > A continuación, se define el `momentum angular del sistema de partículas` con respecto al punto $0$:

$$
\begin{align*}
{\bf{H}}_{0}&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times {\bf{p}}\\
&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times m_{i}{\bf{\dot{r}}}_{i}
\label{eq30}\tag{30}
\end{align*}
$$

+ > Derivando con respecto al tiempo:

$$
\begin{align*}
{\bf{\dot{H}}}_{0}&=\,\sum_{i=1}^{N}\bigg({\bf{\dot{r}}}_{i}\times m_{i}{\bf{\dot{r}}}_{i}+{\bf{r}}_{i}\times m_{i}{\bf{\ddot{r}}}_{i}\bigg)\\
&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times m_{i}{\bf{\ddot{r}}}_{i}\\
&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times {\bf{F}}_i
\label{eq31}\tag{31}
\end{align*}
$$

+ > Llamando a ${\bf{M}}_{0}$ al momento de todas las fuerzas externas en torno a $0$:

$$
\begin{align*}
{\bf{M}}_{0}&=\,\sum_{i=1}^{N}{\bf{r}}_{i}\times {\bf{F}}_i
\label{eq32}\tag{32}
\end{align*}
$$

+ > Se encuentra la misma relación ya conocida: ${\bf{\dot{H}}}_{0}={\bf{M}}_{0}.$

+ > Eso quiere decir que la resultante de todos los momentos en torno al punto fijo $0$, que actuán sobre el sistema de partículas, es igual a la tasa de cambio temporal del momento de momentum en torno a $0$ del todo el sistema.  

+ > Si ahora, se considera el `centro de masa` podemos escribir la fuerza resultante como:

$$
\begin{align*}
{\bf{F}}&=\sum_{i=1}^{N}m_{i}{\bf{\ddot{r}}}_{i}=\sum_{i=1}^{N}m_{i}\bigg({\bf{\ddot{\text{r}}}}_{C}+{\bf{\ddot{\text{r}}}}_{i}^{'}\bigg)\\
&=m\,{\bf{\ddot{\text{r}}}}_{C}+\sum_{i=1}^{N}m_{i}\,{\bf{\ddot{\text{r}}}}_{i}^{'}
\label{eq33}\tag{33}
\end{align*}
$$

+ > Pero sabemos que al trasladar el origen $0$ al `centro de masa`, se cumplirá que:

$$
\begin{align}
\sum_{i=1}^{N}m_{i}\,{\bf{\text{r}}}_{i}^{'}&=0
\label{eq34}\tag{34}
\end{align}
$$

+ > En efecto, se puede demostrar para $N$ partículas:

$$
\begin{align}
{\bf{\text{r}}}_{C}&=\frac{1}{m}\,\sum_{i=1}^{N}m_{i}{\bf{\text{r}_{i}}}\\
&=\frac{1}{m}\,\sum_{i=1}^{N}m_{i}\,({\bf{\text{r}}}_{C}+{\bf{\text{r}}}_{i}^{'})\\
&=\frac{1}{m}\bigg[ \sum_{i=1}^{N}m_{i}\,{\bf{\text{r}}}_{C} + \sum_{i=1}^{N}m_{i}\,{\bf{\text{r}}}_{i}^{'} \bigg]\\
&= {\bf{\text{r}}}_{C}+\frac{1}{m}\sum_{i=1}^{N}m_{i}\,{\bf{\text{r}}}_{i}^{'}
\end{align}
$$

+ > Lo que quiere decir que un centro de masa podría ser definido como aquel punto en el cual se cumple la Ec. ({eq}`34`).

+ > Así que, la fuerza resultante será:

$$
\begin{align*}
{\bf{F}}&=m\,{\bf{\ddot{\text{r}}}}_{C}
\label{eq35}\tag{35}
\end{align*}
$$

```{note}
Hemos demostrado que el movimiento de un sistema de $N$ partículas, bajo la acción de una fuerza resultante ${\bf{F}}$, equivalente a un movimiento de `un solo cuerpo` de masa total $m$, cuya aceleración es aquella del centro de masa ${\bf{\ddot{\text{r}}}}_{C}.$
```

+ > Momentum angular con respecto al centro de masa, se define como:

$$
\begin{align*}
{\bf{H}}_{C}&=\,\sum_{i=1}^{N}{\bf{r}}_{i}^{'}\times m_{i}{\bf{\dot{r}}}_{i}^{'}
\end{align*}
\label{eq36}\tag{36}
$$

+ > Y se puede comprobar que (no se demostrará) que:

$$
\begin{align*}
{\bf{\dot{H}}}_{C}&={\bf{M}}_{C}
\label{eq37}\tag{37}
\end{align*}
$$

+ > Donde se ha usado:

$$
\begin{align*}
{\bf{M}}_{C}&=\,\sum_{i=1}^{N}{\bf{r}}_{i}^{'}\times m_{i}{\bf{F}}_{i}
\label{eq38}\tag{38}
\end{align*}
$$


$$
\begin{align*}
{\bf{\text{F}}}_{i}+\sum_{j=1}^{N}{\bf{f}}_{ji}&=m_{i}\,{\bf{\ddot{r}}}_{i},\quad\quad {\text{i=1,2,}}\ldots{\text{N}} 
\label{eq27}\tag{27}
\end{align*}
$$

+ > Las `Leyes de Newton` se formularon para analizar la dinámica de una sola partícula. Sin embargo, en vibraciones el interés es comprender cuerpos flexibles y que además, ellos pueden oscilar.

+ > `Sistema de partículas`: Vamos a considerar un sistema que consta de $N$ partículas. 

+ > ![Figura Señal2](n_particulas.png)

```{note}
Sistema de $N$ partículas donde la partícula $i$-ésima tiene masa $m_i$.
```

+ > Como se observa en la figura, resulta casi imposible describir con claridad cómo se mueve cada una de las partículas.

```{note}
Entonces para dicho sistema, ¿cómo podemos aplicar nuestro conocimiento acerca de fuerzas, momentos, energía cinética y potencial, y cantidades que se conservan?.
```

+ > `Centro de Masa:` Se dice que cuando el movimiento de un cuerpo flexible implica no sólo `traslación`, sino también `rotación`, o `vibración`, o todas simultáneamente, se debe modelar al cuerpo como si fuese un `sistema de partículas`.

+ > A pesar de lo complejo que pueda resultar todo ese movimiento del sistema, existe un único punto, llamado `Centro de Masa` ($C$), cuyo movimiento de traslación es una característica del sistema como un todo.

+ > Supongamos que tenemos un sistema de solamente dos partículas: $m_1$ y $m_2$ que se mueven en el espacio, con coordenadas $(x_1, y_1, z_1 )$, y $(x_2, y_2, z_2)$. 

+ > Definamos sus vectores de posición como $\vec{r_1}$ y $\vec{r_2}$.

+ > ![Figura CM](C.png)

+ > El centro de masa, $C$, de este sistema se encuentra en algún lugar a lo largo de la línea recta que une las dos masas, con coordenadas $(x_C, y_C, z_C )$. Definimos el vector de posición de $C$ como:

$$
\begin{align*}
\vec{r_C}&= \frac{m_1\cdot \vec{r_1} \,+ \,m_2\cdot \vec{r_2}}{m_1\,+\,m_2} 
\label{eq20}\tag{20}
\end{align*}
$$

+ > Las componentes $x$, $y$ y $z$, del centro de masa son:

$$
\begin{align*}
x_C &= \frac{m_1\cdot x_1 \,+ \,m_2\cdot x_2}{m_1\,+\,m_2} 
\label{eq21}\tag{21}
\end{align*}
$$

$$
\begin{align*}
y_C &= \frac{m_1\cdot y_1 \,+ \,m_2\cdot y_2}{m_1\,+\,m_2} 
\label{eq22}\tag{22}
\end{align*}
$$

$$
\begin{align*}
z_C &= \frac{m_1\cdot z_1 \,+ \,m_2\cdot z_2}{m_1\,+\,m_2} 
\label{eq23}\tag{23}
\end{align*}
$$

## Posición del centro de masa en 1 dimensión para un sistema de dos partículas.

+ > Supongamos un sistema de dos partículas y que conocemos además, sus masas: $m_1=m$ y $m_2=m$.

+ > Las masas se ubican en los puntos $x_1$ y $x_2$ del eje $x$, como se muestra en la figura:

+ > ![Figura CM](2dC.png)

+ > Si la distancia entre las dos partículas la llamamos $D = x_2 - x_1$, y considerando que $y_i=z_i=0,\quad i = 1,2$, tenemos que $y_C =z_C = 0$. 

+ > En consecuencia, la posición del centro de masa en la dimensión $x$ es:

$$
\begin{align*}
x_C &= \frac{m_1\cdot x_1 \,+ \,m_2\cdot x_2}{m_1\,+\,m_2}\\
    &= \frac{m\cdot x_1 \,+ \,m\cdot x_2}{2m}\\
    &= \frac{x_1 \,+ \,x_2}{2}
\label{eq24}\tag{24}
\end{align*}
$$

+ > Pero, usando $x_2= D + x_1$, nos queda: 

$$
\begin{align*}
x_C &= \frac{2x_1 \,+ \,D}{2}\\
    &= x_1 \,+ \, \frac{D}{2}
\label{eq25}\tag{25}
\end{align*}
$$

```{note}
Como demuestra el ejemplo, la posición del centro de masa no coincide necesariamente con la posición de una partícula del sistema.
```

+ > Analizar qué sucede con $x_C$, cuando el origen $0$ del sistema se ubica donde está la partícula $m_1$.

+ > Analizar además, qué ocurre con $x_C$ si la masa de la partícula $m_2$ es igual a $2m$.

+ > Si en este último caso, el origen $0$ del sistema se traslada al centro de masa (es decir, quedando como $0'$), y desde ahí, se miden las distancias a cada una de las masas y se ponderan esas distancias por sus masas respectivas, y luego se suma, entonces qué resultará? Analizar y comentar este resultado.

## Posición del centro de masa en 2 dimensiones para un sistema de tres partículas.

+ > En el siguiente ejemplo, se pide encontrar el centro de masa de un sistema de 3 partículas que tienen cada una, masa $m$ = 1 kg.

+ > ![Figura CM](3masas.png)

## Posición del centro de masa en 3 dimensiones para un sistema de tres partículas.

En el siguiente ejemplo se debe encontrar el centro de masa de un sistema en 3 dimensiones que consta de tres partículas. Las partículas tienen masas $m_1$ = 0,5 ($kg$), $m_2$ = 2 ($kg$) y $m_3$ = 5 ($kg$). Sus posiciones en el espacio son $P_1$(−3,1,2) ($m$), $P_2$(0,1,2) ($m$) y $P_3$(−1,3,0) ($m$), respectivamente.

+ > <img src="3D3masas.png" alt= “” width="350" height="300">

## Posición del centro de masa en 3 dimensiones para un sistema de 8 partículas.

+ > Es más fácil dividir la ecuación vectorial del vector de posición del centro de masa en sus componentes como se ve en las Ecs. ({eq}`21`)-({eq}`23`) y luego, por separado, evaluar cada una de las componentes. Encontrar el centro de masa del siguiente sistema de ocho partículas,  ubicadas en las esquinas de un cubo, todas de igual masa $m$ ($kg$) y separadas una distancia $L$ ($m$), como se muestra en la figura siguiente:

+ > <img src="8m.png" alt= “” width="350" height="300">


<!---
http://www.phys.nthu.edu.tw/~thschang/notes/GP10.pdf

https://repository.kaust.edu.sa/bitstream/handle/10754/666903/system%20of%20particles.pdf?sequence=1&isAllowed=y

https://repository.kaust.edu.sa/bitstream/handle/10754/666903/system%20of%20particles.pdf?sequence=1&isAllowed=y

$$
\begin{align*}
x&=\{x\,[\,n\,]\},\quad \quad -\infty < n < \infty 
\label{eq1}\tag{1}
\end{align*}
$$

<img src="n_particulas.png" alt= “” width="600" height="500">

+ > ![Figura CM](3D3masas.png)

```{note}
Como demuestra el ejemplo, la posición del centro de masa no coincide necesariamente con la posición de una partícula del sistema.
```


## Learn more

This is just a simple starter to get you started.
You can learn a lot more at [jupyterbook.org](https://jupyterbook.org).
-->
