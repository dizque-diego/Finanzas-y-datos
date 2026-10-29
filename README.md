# Finanzas y Datos 
Este es un proyecto con fines educativos cultivando el interés por las finanzas con el fin de desarrollar habilidades en programación en ciencia de datos relacionado con las finanzas.

Este repo funciona como un devlog-portafolio, en el cual la tendencia es desarrollar productos más elaborados e interesantes que simulen eventos del ámbito financiero.
## Proyectos

### 01 - Calculadora de costos
Una calculadora que a partir de datos determinados como la estimación de rentabilidad, el tiempo y costos asociados al activo puede calcular cuánto es el valor de dicho activo después de comisiones.

Aprendí que no solamente es importante tener presente la rentabilidad y el tiempo sino también posibles costos que no se tienen presentes a la hora de invertir o sostener un activo financiero.

Caso concreto: Se invirtió COP $ 351.803 en un fondo colectivo de acciones de estados unidos de la plataforma Trii cuyo TER es del 1.5%, se comparó con el ETF VOO cuyo TER es del 0.03%, usando la misma inversión, misma rentabilidad estimada y mismo tiempo, se encontró que la diferencia después de 20 años es de COP $ 555.445 siendo más rentable VOO. Un activo cuya comisión es tan elevada puede incluso que con el paso del tiempo, el valor de la mera comisión supere el valor de la inversión inicial.
    
### 02 - Simulador Monte Carlo
Va muy de la mano con el proyecto 01, Este simulador Monte Carlo, recoge variables como Tiempo, Rentabilidad estimada y volatilidad y después de hacer 10.000 simulaciones entrega el mejor caso posible, el peor, el promedio y cuál es la posibilidad de perder dinero.

Este ejercicio fue muy enriquecedor puesto que enseño la mecánica de una simulación no muy conocida y darle una funcionalidad con casos de la vida real, como también que aunque la mayoría de los casos sean positivos, es importante tener presente la posibilidad de que las cosas vayan mal.

Como en las primeras simulaciones se encontraron resultados cuya valorización daba en negativo, es decir, como si fuera una deuda -cosa que es imposible- se cambió el modelo de distribución normal por uno a log normal

Caso concreto: Una inversión en el ETF PEPT, con una rentabilidad estimada del 7% y volatilidad del 25%, después de 10 años y 10.000 simulaciones, estimó que de 100 USD invertidos en el mejor de los casos puede llegar a valorizarse hasta USD $2.682, en el peor de los casos hasta 9 y en promedio 197, casi doblar la inversión. Por otro lado el ETF VOO con una rentabilidad del 10% y un 16% de volatilidad, encontró que la posibilidad de perder dinero con la inversión es aproximadamente el 5% de los casos, siendo el peor que el activo termine valiendo USD $37, en promedio se encontró que el activo costaría USD $258 y en el mejor de los casos USD $2.586, si bien es menor rentabilidad que en el ETF PEPT en el mejor de los casos, la probabilidad de perdida de inversión de este último es del 32% aproximadamente frente al 5% de VOO, por lo que siguiendo esta simulación, PEPT es una inversión con un grado de riesgo elevado mientras que VOO es más rentable en promedio y una inversión menos riesgosa.

### 03 - Tracker de portafolio
Este es un sistema que rastrea activos tanto en la Bolsa de valores de USA como en la colombiana, estima cuánto vale cada posición y entrega una consolidación de cuánto vale cada uno de los dos portafolios como también el valor total, en COP y en USD.

Caso concreto: Consolidó acciones de la bolsa de estados unidos y de Colombia y cripto, se unificó el valor a través de la tasa de cambio en COP y USD.

## Tecnologías
- Claude AI (Tutor de aprendizaje)
- Python
- Jupyter Notebook
- NumPy
- yfinance
- Git

## Guía de instalación
1. Clonar el repositorio de este enlace:
```
Git clone https://github.com/dizque-diego/Finanzas-y-datos.git
cd Finanzas-y-datos
```

2. Crear y activar un entorno virtual:
```
python -m venv venv
venv\Scripts\activate
```

3. Instalar dependencias:
```
pip install numpy pandas yfinance jupyter
```

4. Abrir Jupyter y ejecutar cualquiera de los notebooks:
```
jupyter notebook
```


