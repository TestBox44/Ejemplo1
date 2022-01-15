+++
title = "Microservicios en Amazon Web Services"
description = ""
author = ""
date = "2021-11-18"
tags = ["microservicios", "Aplicaciones Web"]
categories = ["Aplicaciones Web", "Arquitecturas"]
[[images]]
  src = "img/2019/03/hp.jpg"
  alt = "Mountain Range Through Clouds"
  stretch = "horizontal"
+++

En este artículo, nos adentraremos en los conceptos de microservicios y sus beneficios, asi como los software que permiten su funcionamiento como funcionalidades independientes.
<!--more-->
## ¿Qué son los microservicios?
Es un enfoque arquitectónico y organizativo para el desarrollo de software, donde este último es compuesto por pequeños servicios independientes que se comunican por APIs definidas.

{{< figure src="/img/postimages/microsvcgraph.png" title="Integración de los microservicios en Aplicación" >}}

## Arquitecturas Monolíticas vs Microservicios
Los microservicios se diseñaron en  respuesta a las arquitecturas monolíticas, la principal caracteristica de estas ultimas era la integración completa de todas las funcionalidades planeadas en una sola aplicación. El problema de este tipo de arquitecturas se encontraba directamente en el riesgo de la disponibilidad por la dependencia de procesos, pues cualquier error no previsto peligraba el funcionamiento completo de la aplicación.
Con los microservicios, cada proceso es independiente y fácilmente escalable.

{{< figure src="/img/postimages/monolith_vs_mcs.png" title="Estructura de las arquitecturas monolíticas vs Microservicios" >}}

## Beneficios de usar microservicios
### Agilidad
Los microservicios fomentan una organización de equipos pequeños e independientes que se apropian de los servicios. Los equipos actúan en un contexto pequeño y bien comprendido, y están facultados para trabajar de forma más independiente y más rápida. Esto acorta los tiempos del ciclo de desarrollo.
### Escalado flexible
Los microservicios permiten que cada servicio se escale de forma independiente para satisfacer la demanda de la característica de la aplicación que respalda. 
### Implementación sencilla
Los microservicios permiten la integración y la entrega continuas, lo que facilita probar nuevas ideas y revertirlas si algo no funciona. El bajo costo de los errores permite experimentar, facilita la actualización del código y acelera el tiempo de comercialización de las nuevas características.
### Libertad tecnológica
Las arquitecturas de microservicios no siguen un enfoque de "diseño único". Los equipos tienen la libertad de elegir la mejor herramienta para resolver sus problemas específicos.
### Código reutilizable
La división del software en módulos pequeños y bien definidos les permite a los equipos usar funciones para diferentes propósitos. 
### Resistencia
La independencia del servicio aumenta la resistencia de una aplicación a los errores. En una arquitectura monolítica, un error en un solo componente, puede provocar un error en toda la aplicación. Con los microservicios, si hay un error en todo el servicio, las aplicaciones lo manejan degradando la funcionalidad sin bloquear toda la aplicación.

## Encapsulamiento y Despliegue de los microservicios

### Docker
Docker es una  plataforma que trabaja con contenedores, los cuales son unidades estándar de software que permitirán el encapsulamiento de los microservicios en imágenes y su ejecución en un entorno informático (servidores o máquinas virtuales).

{{< figure src="/img/postimages/dockerlogo.png" title="" >}}

### Orquestadores
La gestión de los contenedores se da por medio de Orquestadores, los cuales son sistemas que permiten automatizar la implementación, el escalado y la administración de las aplicaciones que se encuentran en los contenedores.
Algunos ejemplos de orquestadores son: Docker Swarm, Kubernetes y Mesos.
{{< figure src="/img/postimages/orquestadores.png" title="" >}}
