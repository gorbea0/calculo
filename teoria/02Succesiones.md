---
title: "Tema 2 - Sucesiones y límites"
author: "Juan Gabriel Gomila, Arnau Mir y Llorenç Valverde"
date: ''
output: 
  ioslides_presentation: 
    css: Mery_style.css
    fig_caption: yes
    keep_md: yes
    logo: Images/calculus.gif
    widescreen: yes
---



# Tema

## Sucesiones

Como hemos visto, el conjunto de los números reales incluye todos los números racionales, es decir, todos los números que tengan un número finito de cifras en su desarrollo decimal. De hecho, también incluye algunos con un número infinito de cifras decimales como seria el caso de los decimales periódicos.

Por consiguiente, los números reales que no son racionales, es decir los números **irracionales** tienen una cantidad infinita de cifras en su desarrollo decimal, tal seria el caso de, por ejemplo $\sqrt{2}$, $\pi$ o $e$.  

Siendo así, ¿cómo podemos utilizar estos números con infinitas cifras decimales? La respuesta viene de la mano del concepto de **sucesión** y de **límite**. 

Cómo hemos demostrado, dado un número irracional y una precisión, siempre es posible determinar un racional que diste del iracional dado menos que dicha precisión. Es lo que hacemos cuando tomamos $\pi$ como $3.14$ o $3.1415$, $\ldots$

## Ejemplos

<div class="example">

**Ejemplo 1.** Consideremos las sucesivas aproximaciones decimales de $\sqrt{2}$,

$$
1,1.4,1.41,1.414,1.4142,1.41421,\ldots
$$ 
Cada uno de estas aproximaciones mejora la anterior, puesto que cada una difiere de $\sqrt{2}$ en menos de $10^{-n}$, donde $n$ indica el número de cifras decimales de la aproximación racional. Obsérvese tambien que una vez alcanzada una determinada precisión, los términos siguientes mejoran dicha precisión.

En general, dado un $\epsilon$, es decir, una precisión, podemos asegurar que, a partir de un término dado que diste menos que esa precisión de la raíz cuadrada de 2, los subsiguientes términos distan de $\sqrt{2}$ menos que esa precisión. .

</div>

<div class="example">

**Ejemplo 2.** Análogamente, las sucesivas aproximaciones decimales del número $\pi$:
$$
3,3.1,3.14,3.141,3.1415,3.14159, \ldots
$$
aproximan el número $\pi$




</div>

## Sucesiones y límites

<l class="definition">Definición</l>

Una **sucesión** $\{a_n \}_{n \in \mathbb{N}}$ de números reales es un conjunto de números reales ordenado según un subíndice que recorre los números naturales. Dicho de una manera más formal, una sucesión de números reales es la imagen de una aplicación del conjunto $\mathbb{N}$ en los reales $\mathbb{R}$.



<div class="example">

**Ejemplos**

**Ejemplo 1. ** Dado un número real $r$, la sucesión constante $a_n = r$, para todo $n \in \mathbb{N}$ es un ejemplo de sucesión. Obsérvese que una sucesión tiene siempre infinitos términos, aunque puedan estar todos o algunos repetidos.

**Ejemplo 2.** La sucesión de término general $a_n = \dfrac{1}{n}$:
$$
1,\dfrac{1}{2},\dfrac{1}{3},\dfrac{1}{4}, \ldots ,\dfrac{1}{n}, \ldots
$$



## Ejemplos de sucesiones

<div class="example">

**Ejemplos**

**Ejemplo 3.** Un ejemplo interesante de sucesión lo constituye la de término general $a_n = 10^{-n}$, és decir la sucesión
$$
0.1,0.01,0.001,0.0001,0.00001, \ldots
$$

**Ejemplo 4.** La sucesión de aproximaciones decimales del número $\pi$: 

 $$
 a_1=3.1\quad a_2=3.14 \quad a_3=3.141 \quad a_4 = 3.1415 \quad a_4 =3.14159 \quad \ldots
 $$

**Ejemplo 5.** Las sucesivas aproximaciones decimales del número $\sqrt{2}$:

$$
a_1=1.4 \quad a_2=1.41 \quad a_3=1.414 \quad a_4=1.4142 \quad a_5=1.41421 \quad \ldots
$$


**Ejemplo 6.** En general, todo número  $\alpha \in \mathbb{R}$, admite un desarrollo decimal en la forma
$$
\alpha= \alpha_0 + \alpha_1 10^{-1}+ \alpha_2 10^{-2}+ \ldots + \alpha_k 10^{-k}+ \ldots 
$$
donde $a_0 \in \mathbb{Z}$ y cada $a_i \in \{0,1,2,\ldots, 9 \}$, de forma que determina una sucesión de término general 
$$
a_n = \alpha_0 + \alpha_1 10^{-1}+ \alpha_2 10^{-2}+ \ldots + \alpha_n 10^{-n} = \alpha_0.\alpha_1\alpha_2\alpha_3\ldots\alpha_n
$$
Obsérvese que para cada $n \in \mathbb{N}$ se tiene que $\alpha-a_n = \alpha_{n+1}10^{-(n+1)}+ \ldots < 10^{-n}$.


</div>


## Sucesiones y límites


<l class="definition">Definición</l>

 
Dada una sucessión $\{a_n\}_{n \in \mathbb{N}}$ de números reales, el número real $a$ és el **límite de la successión dada** si para cada $\epsilon > 0$ existe un lugar $n_0$, a partir del cual todos los términos de la sucesión distan de $a$ menos que $\epsilon$, es decir, si para todo $n \geq n_0$ es 

$$
|a_n -a|< \epsilon 
$$

Escribiremos 

$$
\lim_{n \rightarrow \infty} a_{n} = a \quad \text{ o }  \quad a_n \rightarrow a
$$



## Más ejemplos

<div class="example">

**Ejemplo 3**

$$
\lim_{n \rightarrow \infty}\displaystyle\left\{\frac{1}{n}\right\}_{n \in \mathbb{N}} = 0
$$