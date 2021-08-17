<p align="center">
<img src="http://codeandomexico.org/resources/img/codeandomexico.png" width="500" title="logo_codeando 1 -500">
</p>

[![website](https://img.shields.io/badge/website-CodeandoMexico-00D88E.svg)](http://www.codeandomexico.org/)
[![slack](https://img.shields.io/badge/slack-CodeandoMexico-EC0E4F.svg)](http://slack.codeandomexico.org/)

# Estándar de Datos Abiertos Legislativos

Hola vaquero/a. 🤠 En este proyecto buscamos una forma sencilla para los ciudadanos de saber quién los representa en los congresos locales y federales.

Actualmente si entras a la página de tu congreso local, o del [congreso federal](https://www.congreso.gob.mx) no hay una forma fácil para que una persona identifique quién es su representante. Es necesario saber de geografía electoral para sacar tu distrito local, federal y circunscripción para identificar qué persona te está representando y navegar por portales con una pobre experiencia de usuario (UX). Con este proyecto pretendemos tres cosas:

1. Darle una herramienta sencilla para que todo ciudadano pueda identificar mediante su ubicación quién lo representa y qué está haciendo, así como sus datos de contacto.
2. Mostrarle a los congresos locales y federales que sí se puede lograr una buena experiencia ciudadana a través del diseño de sus herramientas.
3. Proponer un estándar de datos para registrar la actividad legislativa de los congresos locales y federal en una forma unificada.

Para esta misión nos inspiramos grandemente en [Representantes Patito](http://representantes.pati.to/) de [UnRob](https://github.com/unrob) (repo en [GitHub](https://github.com/unRob/representantes.pati.to)). Pero hay otras herramientas que usamos de referencia.

## En qué consiste el proyecto

- Un estándar de datos sobre congresos
- Una API que sirva los datos y en el que se pueda escribir
- Scrappers en el lenguaje de tu preferencia que lean el congreso de tu preferencia para alimentar el API
- Un front que los consuma

## Cómo contribuir

Estamos en la etapa inicial donde se valen todos los perfiles. Queremos que este proyecto sea abierto, asíncrono, remoto y comunitario así que todos son bienvenidos. Siéntete libre de escoger alguna de las siguientes acciones y comunicarte con nosotros via Slack [en el canal del proyecto](https://codeandomexico.slack.com/app_redirect?channel=CLSRKEBQW). Para inscribirte al Slack de Codeando México ve a [este link](http://slack.codeandomexico.org).

Cosas con las que puedes participar:

- Decidiendo un buen nombre
- Haciendo un Logo
- Trabajando en una API
- Diseñando la parte frontal que brinde una buena experiencia de usuario
- Ayudándonos con Project Management
- Recomendando tecnologías para utilizar
- Haciendo recomendaciones sobre cómo identificar y desplegar la información relevante (abogados, politólogos, internacionalistas bienvenidos)

Ayuda que necesitaremos en el futuro:

- Escogiendo un estado de la república mexicana y construyendo un scrapper en el lenguaje de tu preferencia<sup>(1)</sup> para consumir la data 
- Trabajando en el front-end
- Ayudándonos a montar pipelines para la automatización de los scrappers
- Dockerizando

- ¿Se te ocurre alguna otra? escríbenos.

<sup>(1)</sup> Hemos identificado que, además de el diputado y sus datos de contacto, debemos integrar información sobre asistencias, votos, comisiones a las que pertenece y propuestas que ha presentado. Esta es data que habrá que consumir también.

Happy hacking!
