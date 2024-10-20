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
      - [Resultado:](#resultado)
  - [Teorema de Bayes](#teorema-de-bayes)
      - [Fórmula del Teorema de Bayes](#fórmula-del-teorema-de-bayes)
      - [Datos ficticios (del ejemplo anterior):](#datos-ficticios-del-ejemplo-anterior)
      - [Cálculo usando el Teorema de Bayes:](#cálculo-usando-el-teorema-de-bayes)
      - [Resultado:](#resultado-1)
      - [Interpretación:](#interpretación)
  - [Distribución binomial](#distribución-binomial)
  - [Estadística descriptiva](#estadística-descriptiva)
  - [Ley de grandes números](#ley-de-grandes-números)
  - [Teorema central del límite](#teorema-central-del-límite)
  - [Regresiones lineales](#regresiones-lineales)
      - [Alt + 91 para crear corchetes](#alt--91-para-crear-corchetes)
  
  
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

#### Resultado:
La probabilidad condicional de que una persona tenga diabetes, dado que tiene más de 50 años, es aproximadamente **33.33%**.

Esto significa que si ya sabes que una persona es mayor de 50 años, la probabilidad de que esa persona tenga diabetes es del 33.33%, lo cual es mayor que la probabilidad general en la población (14%).

![Probabilidadescondicionales3](assets/Probabilidadescondicionales3.png)
<br>
<br>
![Probabilidadescondicionales4](assets/Probabilidadescondicionales4.png)

---

## Teorema de Bayes

<p>Es utilizado para calcular la probabilidad de un suceso, teniendo información de antemano sobre ese suceso.</p>

El **Teorema de Bayes** nos permite actualizar nuestras creencias sobre un evento con base en nueva información. En este caso, podemos usarlo para calcular la probabilidad de que una persona sea mayor de 50 años, dado que ya sabemos que tiene diabetes.

#### Fórmula del Teorema de Bayes

La fórmula general del teorema es:

$$
P(A|D) = \frac{P(D|A) \cdot P(A)}{P(D)}
$$

Donde:
- \( P(A|D) \) es la probabilidad de que una persona sea mayor de 50 años dado que tiene diabetes.
- \( P(D|A) \) es la probabilidad de que una persona tenga diabetes dado que es mayor de 50 años.
- \( P(A) \) es la probabilidad de que una persona sea mayor de 50 años.
- \( P(D) \) es la probabilidad de que una persona tenga diabetes.

#### Datos ficticios (del ejemplo anterior):
- **Probabilidad de tener diabetes dado que la persona es mayor de 50 años**: \( P(D|A) = 0.3333 \) (33.33%).
- **Probabilidad de que una persona tenga más de 50 años**: \( P(A) = 0.30 \) (30%).
- **Probabilidad de que una persona tenga diabetes**: \( P(D) = 0.14 \) (14%).

#### Cálculo usando el Teorema de Bayes:

Sustituyendo los valores en la fórmula:

$$
P(A|D) = \frac{0.3333 \times 0.30}{0.14} = \frac{0.09999}{0.14} \approx 0.714
$$

#### Resultado:
La probabilidad de que una persona sea mayor de 50 años, dado que tiene diabetes, es aproximadamente **71.4%**.

#### Interpretación:
El **Teorema de Bayes** nos ayuda a calcular la probabilidad inversa. En este caso, mientras que inicialmente solo sabíamos la probabilidad de que alguien tenga diabetes dado que es mayor de 50 años, ahora podemos calcular la probabilidad de que alguien sea mayor de 50 años dado que tiene diabetes. Según nuestros cálculos, si una persona tiene diabetes, hay un 71.4% de probabilidad de que tenga más de 50 años.



## Distribución binomial
Aquí va el contenido de la sección de la distribución binomial.
> esta es una nota

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

#### Alt + 91 para crear corchetes
![EquiposScrum](assets/EquiposScrum.png "Titulo de la imagen")


Reglas github
* [x]  tarea 1
* [x]  tarea 2
* [ ]  tarea 3
  


[def]: assets/Probabilidadescondicionales4.png