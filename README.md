# Salesforce Spring ’18 Assessment
El objetivo de este proyecto es describir los requisitos básicos de una aplicación desarrollada
bajo [Salesforce](http://www.salesforce.com).
El desarrollo de la aplicación permite evaluar las capacidades técnicas del desarrollador :)

Dicho de otra manera: este proyecto es el guión de un test.

## dTakers School. Caso de uso

![dTakers School](http://github.com/dtakers/salesforce-spring18-assessment/dtakers_school.png)

Eres el nuevo administrador de dTakers School, un centro educativo líder en enseñanza relacionada con las tecnologías de la información.

El director dTakers School te ha dado la bienvenida al equipo y te ha comentado la necesidad de desarrollar una aplicación que permita gestionar todo el catálogo de formación del centro.

El centro dispone de varias aplicaciones en Salesforce con las que gestionan las relaciones con otros centros, por lo que el director te indica que necesitan una nueva [App](http://sforce.co/2HKlZoP) para Salesforce Lightning Experience.

El director confía en tu experiencia y capacidad, por lo que dispones de total libertad para desarrollar la App.

El director te comenta por encima de que forma les gustaría trabajar con la App:

- Al inicio del año los profesores se reunirán con el director y establecerán la oferta educativa. Como mínimo existirá un curso, un taller, un seminario, una experiencia nacional y una experiencia internacional
- Se decidirá que profesor será responsable de cada opción. Un profesor puede ser responsable de varias opciones.
- Una vez que se ha decidido qué profesor será responsable, la App automáticamente creará una tarea para que el departamento de contabilidad calcule el precio de venta y el coste por alumno
- Los alumnos contactarán con dTakers School vía telefónica o email, y el personal de administración incluirá a los alumnos en la opción solicitada, salvo que no queden plazas libres  

En dTakers School disponen de la siguiente oferta educativa:

- Cursos: son siempre de duración determinada, entre dos fechas dadas. El título debe incluir **automáticamente** la fecha de inicio y la fecha de fin
- Talleres: son siempre de duración determinada (1, 2 o 3 días). El título debe incluir **automáticamente** el número de días de duración
- Seminarios: son siempre de duración determinada y fija (4 días).
- Experiencias nacionales e internacionales: son siempre de duración determinada y fija (1 día)

Cualquier opción de la oferta educativa tiene en común las siguientes características:

- Título
- Número limitado de asistentes
- Fechas de inicio y fin
- Un profesor
- Precio de venta por alumno
- Coste por alumno

dTakers School necesita una solución que tenga en cuenta a las siguientes personas:

- Alumnos: no son usuarios de Salesforce. Son personas que solicitan (vía teléfonica o email) cualquier opción de la oferta educativa. Como mínimo debe guardarse: nombre y apellidos, teléfono de contacto y email. Hay que tener en cuenta la LOPD y el RGPD
- Administrativos: son usuarios de Salesforce que dan de alta a los alumnos en las distintas opciones de la oferta educativa, pero no gestionan la oferta educativa
- Profesores: son usuarios de Salesforce que gestionan la oferta educativa (alta, modificación, baja...) pero no gestionan a los alumnos
- Contabilidad: son usuarios de Salesforce. Son los únicos usuarios que pueden ver y gestionar el coste por alumno. El resto de datos solo pueden consultarse por este usuario 

## ¿Qué vamos a valorar?

Por encima de todo, el objetivo es que la aplicación funcione conforme a lo indicado por le director de dTakers School. Nosotros valoraremos también:

- El modelo de datos debe ajustarse a la solución. Número de objetos, tipo, relaciones, nombres y campos
- Seguridad acorde con lo indicado. Perfiles, seguridad a nivel campos y visibilidad de la información
- La App debe resolver correctamente el problema planteado
- La App debe estar personalizada correctamente
- El código desarrollado (si se ha desarrollado algo) debe entenderse fácilmente y estar documentado correctamente
- Los Test deben verificar al menos el 80% del código desarrollado (en el caso de haber desarrollado código)
- La App debe poder instalarse sin problemas en cualquier organización de tipo Developer de Salesforce (puedes usar 2GP)

## ¿Cómo lo vamos a valorar?

| Área| Valor |
| ------ | ------ |
| Modelo de datos | 20% |
| Seguridad | 5% |
| Desarrollo App | 35% |
| Personalización App | 5% |
| Código APEX | 10% |
| Tests unitarios | 10% |
| Empaquetado e instalación | 15% |

## Opcionalmente (puede ayudar en la valoración ;) )
No es obligario, pero puede ayudarnos en la valoración:

- Uso de Git
- Uso de Einstein
- Uso de Reports y Dahsboards
- Integración con otros sistemas de información externos a Salesforce

## Licencia
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/">
	<img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" />
</a><br />
<span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Salesforce Spring '18 Assessment</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://www.dtakers.com" property="cc:attributionName" rel="cc:attributionURL">Digital Takers S.L.</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.<br />
Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="http://github.com/dtakers/salesforce-spring18-assessment" rel="dct:source">http://github.com/dtakers/salesforce-spring18-assessment</a>.