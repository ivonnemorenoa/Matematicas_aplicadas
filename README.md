# Estadísticas



## Índice

- [Estadísticas](#estadísticas)
  - [Índice](#índice)
  - [Probabilidades condicionales](#probabilidades-condicionales)
    - [Ejemplo: Probabilidad de tener diabetes dado que la persona es mayor de 50 años](#ejemplo-probabilidad-de-tener-diabetes-dado-que-la-persona-es-mayor-de-50-años)
      - [Información ficticia:](#información-ficticia)
      - [Queremos calcular:](#queremos-calcular)
      - [Fórmula de la probabilidad condicional:](#fórmula-de-la-probabilidad-condicional)
      - [Sustituimos los valores:](#sustituimos-los-valores)
  - [Teorema de Bayes](#teorema-de-bayes)
      - [Fórmula del Teorema de Bayes](#fórmula-del-teorema-de-bayes)
      - [Datos ficticios (del ejemplo anterior):](#datos-ficticios-del-ejemplo-anterior)
      - [Cálculo usando el Teorema de Bayes:](#cálculo-usando-el-teorema-de-bayes)
    - [Forma extendida](#forma-extendida)
  - [Distribución binomial](#distribución-binomial)
      - [Características de la distribución binomial](#características-de-la-distribución-binomial)
    - [Fórmula de la Distribución Binomial](#fórmula-de-la-distribución-binomial)
  - [Estadística descriptiva](#estadística-descriptiva)
  - [Ley de grandes números](#ley-de-grandes-números)
  - [Teorema central del límite](#teorema-central-del-límite)
  - [Regresiones lineales](#regresiones-lineales)
      
      
  
  
## Probabilidades condicionales

<p>Es la posibilidad de que ocurra un evento, al que denominamos A, como consecuencia, de que ha tenido lugar otro evento, al que denominamos B.</p>

> ### Puntos clave
> * Mide la probabilidad de que ocurra algo (A) despues de que ya ha ocurrido otra cosa distinta (B).<br>
> <br>
> * A diferencia de la probabilidad independiente, en la condicional, la ocurrencia de un evento sí afecta la probabilidad del otro.<br>
> <br>
> * Su fórmula es: P(A|B) = P(A ∩ B) / P(B). Dividir entre cero siempre nos va a traer problemas.<br>
> <br>

<p>Lo que queremos calcular es la probabilidad de que ocurra el evento A dado que ha ocurrido B. Es seguro que ha ocurrido B, sí o sí.</p>

![Probabilidadescondicionales1](assets/Probabilidadescondicionales1.png)

Entonces estaremos concentrados solo en la intersección.<br>

![Probabilidadescondicionales2](assets//Probabilidadescondicionales2.png)

> Formula de la probabilidad:
$$
P(A) = \frac{\text{Número de casos favorables}}{\text{Número total de casos posibles}}
$$
### Ejemplo: Probabilidad de tener diabetes dado que la persona es mayor de 50 años

Supongamos que estamos analizando datos sobre la población mexicana y queremos calcular la probabilidad condicional de que una persona tenga diabetes, dado que ya sabemos que la persona tiene más de 50 años.

#### Información ficticia:
- **Probabilidad de que una persona en México tenga diabetes**: \( P(D) = 0.14 \) (14% de la población tiene diabetes).
- **Probabilidad de que una persona tenga más de 50 años**: \( P(A) = 0.30 \) (30% de la población tiene más de 50 años).
- **Probabilidad de que una persona tenga diabetes y sea mayor de 50 años**: \( P(D ∩ A) = 0.10 \) (10% de la población tiene diabetes y es mayor de 50 años).

#### Queremos calcular:
La **probabilidad condicional** de que una persona tenga diabetes dado que ya sabemos que tiene más de 50 años, es decir, \( P(D | A) \).

#### Fórmula de la probabilidad condicional:

$$
P(D | A) = \frac{P(D \cap A)}{P(A)}
$$

Donde:
- \( P(D | A) \) es la probabilidad de tener diabetes dado que la persona tiene más de 50 años.
- \( P(D ∩ A) \) es la probabilidad de que la persona tenga diabetes y sea mayor de 50 años.
- \( P(A) \) es la probabilidad de que la persona tenga más de 50 años.

#### Sustituimos los valores:

$$
P(D | A) = \frac{0.10}{0.30} = 0.3333
$$

Resultado:<br>
La probabilidad condicional de que una persona tenga diabetes, dado que tiene más de 50 años, es aproximadamente **33.33%**.

Esto significa que si ya sabes que una persona es mayor de 50 años, la probabilidad de que esa persona tenga diabetes es del 33.33%, lo cual es mayor que la probabilidad general en la población (14%).

![Probabilidadescondicionales3](assets/Probabilidadescondicionales3.png)
<br>
<br>
![Probabilidades](assets/Probabilidadescondicionales4.png)

---

## Teorema de Bayes

<p>Es utilizado para calcular la probabilidad de un suceso, teniendo información de antemano sobre ese suceso.</p>

El **Teorema de Bayes** nos permite actualizar nuestras creencias sobre un evento con base en nueva información. En este caso, podemos usarlo para calcular la probabilidad de que una persona sea mayor de 50 años, dado que ya sabemos que tiene diabetes.

#### Fórmula del Teorema de Bayes

La fórmula general del teorema es:

$$
P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}
$$

Donde:
- \( P(A|B) \) es la probabilidad de que una persona sea mayor de 50 años dado que tiene diabetes.
- \( P(B|A) \) es la probabilidad de que una persona tenga diabetes dado que es mayor de 50 años.
- \( P(A) \) es la probabilidad de que una persona sea mayor de 50 años.
- \( P(B) \) es la probabilidad de que una persona tenga diabetes.

#### Datos ficticios (del ejemplo anterior):
- **Probabilidad de tener diabetes dado que la persona es mayor de 50 años**: \( P(B|A) = 0.3333 \) (33.33%).
- **Probabilidad de que una persona tenga más de 50 años**: \( P(A) = 0.30 \) (30%).
- **Probabilidad de que una persona tenga diabetes**: \( P(B) = 0.14 \) (14%).

#### Cálculo usando el Teorema de Bayes:

Sustituyendo los valores en la fórmula:

$$
P(A|B) = \frac{0.3333 \times 0.30}{0.14} = \frac{0.09999}{0.14} \approx 0.714
$$

Resultado:<br>
La probabilidad de que una persona sea mayor de 50 años, dado que tiene diabetes, es aproximadamente **71.4%**. <br>

Otros ejemplos a continuacion:<br>

![](assets/TeoremadeBayes.png)
<br>
<br>
![](assets/TeoremadeBayes2.png)
<br>
<br>
![](assets/TeoremadeBayes3.png)
<br>

### Forma extendida
C.E.: Colectivamente exahustivos. <br> 
M.E.: mutuamente excluyentes. <br>
Partición del espacio muestral. <br>

![](assets/TeoremadeBayes5.png)
<br>

## Distribución binomial

Las Matematicas nos dicen que el orden de los factores no alteran el producto.<br>

¿Que es la distribución binomia?<br>
<p>
Es un modelo de probabilidad que describe el número de éxitos en una serie de ensayos independientes de tipo "éxito o fracaso", donde cada ensayo tiene la misma probabilidad de éxito. Es útil para situaciones donde hay solo dos posibles resultados, como "sí" o "no", "verdadero" o "falso", "aprobado" o "reprobado".
</p>

#### Características de la distribución binomial

Para que una situación se modele con una distribución binomial, debe cumplir con los siguientes criterios:<br>

1. Número fijo de ensayos 𝑛: La situación involucra un número específico de intentos o ensayos.
2. Resultados binarios: Cada ensayo tiene solo dos resultados posibles (éxito o fracaso).
3. Probabilidad constante de éxito 𝑝: La probabilidad de éxito es la misma para cada ensayo.
4. Independencia: Los resultados de cada ensayo no afectan a los demás.

### Fórmula de la Distribución Binomial

La fórmula para calcular la probabilidad de obtener exactamente \( k \) éxitos en \( n \) ensayos es:

$$
P(X = k) = \binom{n}{k} p^k (1 - p)^{n - k}
$$

Donde:
- \( P(X = k) \) es la probabilidad de obtener \( k \) éxitos.
- \( n \) es el número total de ensayos.
- \( k \) es el número de éxitos deseados.
- \( p \) es la probabilidad de éxito en cada ensayo.
- \( 1 - p \) es la probabilidad de fracaso.

El *coeficiente binomial* \( \binom{n}{k} \), también conocido como "combinaciones de \( n \) en \( k \)", se calcula como:

$$
\binom{n}{k} = \frac{n!}{k!(n - k)!}
$$
<br>

![](assets/binomial.png)
<br>
![](assets/binomial2.png)
<br>
> Tenemos valores enteros y mayores o iguales que 0. La Distribución Binomial es una distribución de probabilidad D i s c r e t a, no continua.
<br>

> Estudiar Distribución de Poison y no confundir.

![](assets/binomial3.png)

<br>

> No olvidar la variable aleatoria binomial que es la X mayúscula.

[Clase explicativa a YouTube](https://www.youtube.com/watch?v=HJgJGYDXojk&list=PL3KGq8pH1bFRKK6-4DHifbjLtnif-O7eW&index=2)

> N Factorial, representado como **n!**, es el producto de todos los números enteros positivos que hay entre el número n y el 1, ej. 4! = 4 * 3 * 2 * 1 = 24   
> NOTA: 0! es igual a 1

**Solución "a"**

![](assets/binomial4.png)
<br>

**Solucion "b"**

![](assets/binomial5.png)

<br>

## Estadística descriptiva
Aquí va el contenido de la sección de estadística descriptiva.
> esta es una nota

## Ley de grandes números
Aquí va el contenido de la sección de la ley de grandes números.
> esta es una nota

## Teorema central del límite
Aquí va el contenido de la sección del teorema central del límite.
> esta es una nota

## Regresiones lineales
Aquí va el contenido de la sección de regresiones lineales.
> esta es una nota



`
Codigo
    escrrito
    para programadores
    que
necesita codigo
`

```python
print("hello world")
```

| Table | Are   | Cool  |
|-------|-------|-------|
| Mesa  | es    | chida |
| quiero| comer | carne |
|       |       |       |

  


