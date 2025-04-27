# Estudio de las Deudas Registradas del Sistema Financiero Argentino

## Descripción del repositorio

Este repositorio contiene el trabajo práctico de la materia Introducción a Data Mining de la Maestría en Ciencia de Datos de la Universidad Austral.

El objetivo del trabajo fue analizar y modelar una base de datos relacionada con las deudas registradas en el sistema financiero argentino, aplicando técnicas de reducción de dimensionalidad, clustering y modelos de clasificación.

## Contexto de los datos

El Banco Central de la República Argentina (BCRA) publica mensualmente un informe denominado "Central de Deudores del Sistema Financiero", el cual consolida información de las deudas actuales e históricas (últimos 24 meses) de personas físicas y jurídicas. Esta información es elaborada a partir de los datos provistos por:

- Entidades financieras

- Empresas no financieras emisoras de tarjetas de crédito

- Fideicomisos financieros

- Otros proveedores no financieros de crédito

Cada deuda registrada es acompañada de su situación crediticia, definida como:

- Situación 1 | Situación normal: atraso en el pago que no supere los 31 días.

- Situación 2 | Riesgo bajo: atraso en el pago de más de 31 días y hasta 90 días.

- Situación 3 | Riesgo medio: atraso en el pago de más de 90 días y hasta 180 días.

- Situación 4 | Riesgo alto: atraso en el pago de más de 180 días a un año.

- Situación 5 | Irrecuperable: atraso superior a un año.

- Situación 6 | Irrecuperable por disposición técnica: deuda con una ex entidad.

## Descripción de la muestra

Se trabajó con una muestra aleatoria de 19.737 CUITs correspondientes a personas físicas que, en junio de 2019, cumplían tres condiciones específicas: tener al menos una deuda registrada en el sistema financiero, encontrarse en situación crediticia 1 o 2 (es decir, sin atrasos mayores a 90 días) y poseer un monto total adeudado inferior a 100.000 pesos argentinos. Para cada uno de estos CUITs, se registraron y resumieron las deudas existentes en junio de 2019 y en los seis meses previos. Además, se recolectó información sobre las deudas correspondientes al período comprendido entre julio de 2019 y junio de 2020, con el objetivo de analizar su evolución a lo largo del tiempo.

## Actividades realizadas

El análisis realizado incluyó la aplicación de técnicas de reducción de dimensionalidad para condensar la información relevante de la base de datos, disminuyendo su complejidad sin perder capacidad explicativa. Posteriormente, se efectuó una segmentación de los deudores mediante técnicas de clustering, agrupándolos en conjuntos homogéneos según su comportamiento crediticio. Finalmente, se desarrollaron modelos de clasificación utilizando Random Forest, con el fin de predecir la evolución de la situación crediticia de los deudores en el tiempo.
