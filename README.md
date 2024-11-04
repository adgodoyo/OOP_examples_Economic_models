# OOP Examples for Economic Models / Ejemplos de POO para Modelos Económicos

## English Version

### Repository Overview

This repository contains examples of Python code developed at Universidad Externado to practice **Object-Oriented Programming (OOP)** concepts in the context of economic models. Each file represents an economic model encapsulated in a Python class, allowing users to instantiate objects with specific values and perform various economic calculations.

The main goal of this project is to teach students how to implement classes and objects in Python while learning about economic theories and their mathematical formulations. This approach helps reinforce OOP programming.

### Available Models

The repository includes implementations of the following economic models:

1. **Phillips Curve**: Demonstrates the inverse relationship between inflation and unemployment. The code implements methods to calculate inflation based on different unemployment rates and allows graphical representations.
   
2. **Price Discrimination**: Implements a model for price discrimination, showing how firms with market power set different prices for different consumer groups.

3. **IS-LM Model**: A macroeconomic model representing the relationship between the interest rate (I) and the supply of money (LM) in an economy.

4. **Stackelberg and Perfect Competition**: Simulates the Stackelberg model of oligopoly and compares it with perfect competition.

5. **Dutch and English Auction**: Models two types of auctions and their respective mechanisms, explaining how the pricing process works.

6. **Mundell-Fleming Model**: Describes an open economy under different exchange rate regimes and the interaction between fiscal and monetary policy.

### Example of a Model: Phillips Curve

The Phillips Curve model, which is widely used in macroeconomic theory, can be instantiated and used as follows:

```python
class CurvaPhillips:
    def __init__(self, inflacion_esperada, nairu, beta):
        self.inflacion_esperada = inflacion_esperada
        self.nairu = nairu
        self.beta = beta

    def calculo_inflacion(self, desempleo, choque=0):
        inflacion = self.inflacion_esperada - self.beta * (desempleo - self.nairu) + choque
        return inflacion

# Creating an instance of the Phillips Curve
curva = CurvaPhillips(inflacion_esperada=2, nairu=5, beta=0.5)
print(curva.calculo_inflacion(desempleo=6))
```

This code defines the Phillips Curve as a class with methods to calculate inflation given specific parameters like the unemployment rate and expected inflation.

### Installation and Requirements

To run these models, you will need:

- Python 3.x
- Jupyter Notebook (or another Python IDE)
- Libraries: matplotlib (for graphs)

You can install the necessary libraries using pip, for example:

```bash
pip install matplotlib
```

---

## Versión en Español

### Resumen del Repositorio

Este repositorio contiene ejemplos de código en Python desarrollados en la clase de Programación en la Universidad Externado para practicar conceptos de **Programación Orientada a Objetos (POO)** en el contexto de modelos económicos. Cada archivo representa un modelo económico encapsulado en una clase de Python, permitiendo a los usuarios instanciar objetos con valores específicos y realizar cálculos económicos.

El objetivo principal de este proyecto es enseñar a los estudiantes cómo implementar clases y objetos en Python, mientras aprenden sobre teorías económicas y sus formulaciones matemáticas. Este enfoque refuerza los conceptos teóricos de economía mediante la practica de Programación de Orientada a Objetos.

### Modelos Disponibles

El repositorio incluye implementaciones de los siguientes modelos económicos:

1. **Curva de Phillips**: Demuestra la relación inversa entre la inflación y el desempleo. El código implementa métodos para calcular la inflación en función de diferentes tasas de desempleo y permite la representación gráfica.

2. **Discriminación de Precios**: Implementa un modelo de discriminación de precios, mostrando cómo las empresas con poder de mercado establecen diferentes precios para distintos grupos de consumidores.

3. **Modelo IS-LM**: Un modelo macroeconómico que representa la relación entre la tasa de interés (I) y la oferta monetaria (LM) en una economía.

4. **Oligopolio de Stackelberg y Competencia Perfecta**: Simula el modelo de Stackelberg de oligopolio y lo compara con la competencia perfecta.

5. **Subasta Holandesa e Inglesa**: Modela dos tipos de subastas y sus respectivos mecanismos, explicando cómo funciona el proceso de precios.

6. **Modelo Mundell-Fleming**: Describe una economía abierta bajo diferentes regímenes de tipo de cambio y la interacción entre la política fiscal y monetaria.

### Ejemplo de un Modelo: Curva de Phillips

El modelo de la Curva de Phillips, ampliamente utilizado en la teoría macroeconómica, puede instanciarse y usarse de la siguiente manera:

```python
class CurvaPhillips:
    def __init__(self, inflacion_esperada, nairu, beta):
        self.inflacion_esperada = inflacion_esperada
        self.nairu = nairu
        self.beta = beta

    def calculo_inflacion(self, desempleo, choque=0):
        inflacion = self.inflacion_esperada - self.beta * (desempleo - self.nairu) + choque
        return inflacion

# Crear una instancia de la Curva de Phillips
curva = CurvaPhillips(inflacion_esperada=2, nairu=5, beta=0.5)
print(curva.calculo_inflacion(desempleo=6))
```

Este código define la Curva de Phillips como una clase con métodos para calcular la inflación dadas las variables como la tasa de desempleo y la inflación esperada.

### Instalación y Requisitos

Para ejecutar estos modelos, necesitarás:

- Python 3.x
- Jupyter Notebook (o cualquier IDE de Python)
- Librerías: matplotlib (para gráficos)

Puedes instalar las librerías necesarias usando pip:

```bash
pip install matplotlib
```
