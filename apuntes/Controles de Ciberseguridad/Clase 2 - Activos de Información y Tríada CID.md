
## Tríada CID 🔺

La tríada CID corresponde a 3 propiedades de la seguridad, sirven para establecer controles e incidentes:
- Confidencialidad: La información solo puede ser accedida por personal autorizado previamente.
- Integridad: La información debe mantenerse intacta, incorrupta y sin modificaciones desde su origen hasta su destino.
- Disponibilidad: La información debe estar disponible cuando sea requerida.

### Ejemplos de incidentes: 
- Incidente de confidencialidad: Al acceder a mi correo electrónico, puedo ver los correos de otro usuario, este incidente afecta directamente a la confidencialidad 
- Incidente de integridad: Califico a un estudiante con una nota en el sistema, y cuando el estudiante la revisa, aparece otra que no corresponde.
- Incidente de disponibilidad: Se corta el servicio de internet y no puedo acceder a la información, se encuentra caída la página, etc

### Ejemplos de controles de seguridad:
- Control de confidencialidad: Autentificación para acceder a la información
- Control de integridad: Firma digital o hash para verificar que la información no ha sido alterada
- Control de disponibilidad: Sistemas redundantes o respaldos para garantizar acceso continuo

![[cubo.png]]

### Volviendo a los activos...
1. En primera instancia, el diagrama comienza desde activo, existe un activo.
2. Luego, un activo puede estar propenso a una amenaza.
3. Esta amenaza normalmente se da porque surge a través de un riesgo
4. Un riesgo surge debido a que puede existir una vulnerabilidad en el sistema

![[activos.png]]

## ¿Qué es un riesgo?
Es la posibilidad de que ocurra un acontecimiento que tenga un impacto (tanto positivo como negativo) ISO 31.000

Riesgo = Impacto x Probabilidad

Impacto: son las consecuencias que se podrían generar como consecuencia del evento
Probabilidad: es la posibilidad de que el evento ocurra.

Ejemplo: Un funcionario está a cargo de un laboratorio de computación en una institución educacional, este laboratorio está cerca de los baños del piso.
1. ¿Qué riesgos corre el funcionario? 
	- Que ocurra un derrame en el piso que pueda afectar la parte eléctrica del laboratorio
	- Que no tenga respaldo de la información
	- Que entre un malware a la red

El funcionario toma conciencia de estos riesgos por lo que hala con el prevencionista de riesgos de la institución, como el encargado de informática y redes. Expone la información por lo que el prevencionista entrega un informe detallado de los riesgos. Para esto, se evalúan soluciones de backup, HA, antivirus, etc.

Ahora el funcionario cuenta con una política de respaldo, mejor ubicación y evitando un accedo de malware ya que se encuentra separada de la red organizacional.

## Mitigación de Riesgos
Para mitigar riesgos, se implementan controles

![[interrelaciones.png]]

## Activos en el ciberespacio
### Activos personales:
Suscripciones en línea, identidad en linea del consumidor individual, datos médicos, cuenta bancaria, cuentas de correo electrónico, fotos, vídeos música, etc.

- Activos físicos: Dispositivos como computadoras, smartphones, tabletas, etc.
- Activos virtuales: Contenidos digitales, cuentas online, identidad digital, etc.

### Activos de la organización
- Activos físicos: Servidores, equipos de red, dispositivos de almacenamiento, etc.
- Activos virtuales: Aplicaciones, datos corporativos, propiedad intelectual digital, etc.

## Activo crítico
Un activo crítico es cuando tiene el POTENCIAL de impactar significativamente el logro de los objetivos de la organización.
Si tenemos dos activos, debemos identificar cuál tiene mayor criticidad para implementar controles más estrictos y asignar recursos de protección de manera prioritaria.

## Amenazas
Según ISO 27.032, cláusula 4.46: Causa potencial de un incidente no deseado, que puede resultar en daño a un sistema, un individuo u organización

## Incidente vs Ataque

> [!info] Es importante identificar que un incidente es distinto de un ataque, por ejemplo, hay un cable que es movido por un trabajador y se desconecta. El sistema se cae. Esto representa un incidente pero no necesariamente un ataque.

## Agente de amenaza
Es un individuo o grupo de individuos que tienen un rol en la ejecución o respaldo sobre un ataque

## Vulnerabilidad
ISO 27.032
La debilidad de un activo o de un control que pueda ser explotada por una amenaza

> [!info] Un sistema nunca tendrá vulnerabilidad cero, siempre puede existir un grado de vulnerabilidad

CVE - Common Vulnerabilities and Exposures
Muestran las vulnerabilidades más comunes

CWE - Common Weakness Enumeration
Muestran las debilidades más comunes

## Diferencia entre vulnerabilidad vs debilidad
"Una vulnerabilidad es la manifestación de una o más debilidades en un sistema" Por lo que, una vulnerabilidad puede abarcar una o más debilidades en el sistema. Un conjunto de debilidades puede conformar una vulnerabilidad.

Ejemplos de debilidad
CWE-89 SQL Injection
Es una debilidad en la cual se realizan consultas a la base de datos a través de inyección de peticiones en formato SQL

Ejemplos de vulnerabilidad
CVE 2021-4428
contiene distintas debilidades relacionadas a validaciones de inputs

## Tipos de vulnerabilidades
Según la ISO 27.005, Anexo D (Riesgos de las TI)
1. Hardware
	Ejm: mantenimiento insuficiente, portabilidad
2. Software
	Ejm: no hay registros de inscripción, interfaz complicada de utilizar
3. Red
	Ejm: Falta de encriptación en transferencias en red, único punto de acceso disponible
4. Personal
	Ejm: formación insuficiente, falta de supervisión de parte del personal
5. Sitio
	Ejm: sistema eléctrico inestable, sitio en área susceptible a inundaciones
6. Estructura de la organización
	Ejm: falta de separación de tareas, no hay descripción de los puestos de la organización

## Tipos de Amenazas 

![[Pasted image 20250301084043.png]]
## Riesgo
Según la ISO 27.005, cláusula 3.9 e ISO 27.000, cláusula 2.68

- El riesgo es el efecto de la incertidumbre en los objetivos, es la combinación de las consecuencias de un suceso de seguridad de la información y la probabilidad de que ocurra.

> [!info] Probabilidad (Frecuencia) x Consecuencia (Impacto) = Riesgo

Para evitar los riesgos, se deben implementar controles
## Clasificación de Controles

- Control preventivo: se implementar para desalientar o prevenir la aparición de problemas. Ejm: hardening, autenticación de múltiples factores, cifrado de datos sensibles.
- Control de detección: se implementan para buscar, detectar e identificar problemas. Ejm: monitoreo y revisión de logs, scanner de vulnerabilidades 
- Control correctivo: se implementan para resolver problemas encontrados y prevenir que vuelvan a ocurrir. Ejm: restaurar datos de copias de seguridad, aislamiento de sistemas afectados para evitar propagación, análisis forense

## Programa de Ciberseguridad
Para establecer y administrar un programa de ciberseguridad este incluye todas las partes relevantes que trabajarán conjuntamente para proteger la inversión de la compañía en relación al hardware y sistemas de software y que asegurarán la CID (Confidencialidad, Integridad y Disponibilidad) de la información.

Para crear este programa de ciberseguridad se debe tener en cuenta tamaño, complejidad y sensibilidad de la información de la empresa.

### Componentes de un programa de ciberseguridad:
1. Gobierno de seguridad: políticas, estándares y procedimientos
2. Evaluación de riesgos y gestión de vulnerabilidades
3. Gestión de accesos e identidades
4. Seguridad de la infraestructura y aplicaciones
5. Respuesta a incidentes y continuidad del negocio
6. Concientización y capacitación del personal
7. Monitoreo y auditoría de seguridad
8. Cumplimiento regulatorio y legal

## Marco de ciberseguridad
Es un conjunto de directrices, estándares, buenas prácticas y/o procedimientos para gestionar los riesgos de seguridad.
Ofrece una base sólida para construir tu plan director de ciberseguridad.

Es importante tener en mente las sgtes preguntas:
- Postura actual de la ciberseguridad
- Estado deseado para la ciberseguridad
- Objetivos que se desean alcanzar
- Oportunidades para mejorar
- Evaluar el progreso hacia el estado deseado
- Riesgo de ciberseguridad
- Requisitos de legislación
- Requisitos de la norma
- Requisitos contractuales
- Beneficios que se desean obtener

Por ejemplo, si estamos en una empresa bancaria, esta no se regirá de igual forma que una empresa que vende productos en internet. Deben cumplir con distintos niveles o estados de seguridad y cumplir con las leyes dependiendo de como operan.
## NIST
Es un marco publicado por el Instituto Nacional de Estándares y Tecnología (National Institute of Standards and Tecnlology) Esta guía cubre las prácticas esenciales 
Funciones principales:
- Proteger 
- Recuperar
- Identificar
- Detectar
- Responder
- Gobierno

NIST no es certificable como ISO


## CIS Control v8
Es un conjunto de 18 controles, en donde cada uno tiene subcontroles.

A nivel organizacional se recomienda CIS Control debido a que es adaptable al tamaño de la organización, principalmente para empresas pequeñas o que están surgiendo.

Primero, CIS Control realiza una autoevaluación para identificar el nivel en el que se encuentra la organización.

## ENISA
Enisa: European Union Agency for Cibersecurity
Es un marco europeo que tiene regulaciones europeas específicas para la protección de infraestructuras críticas y servicios esenciales dentro de la Unión Europea.

## ENS
ENS: Esquema Nacional de Seguridad
Es un framework que se aplica al sector público que tiene requisitos para la protección de la información. Categoriza los sistemas en función a las dimensiones que puede tener:
Le suma autenticidad y trazabilidad a la tríada de la seguridad:
- Confidencialidad
- Integridad
- Disponibilidad
- Autenticidad: Garantía de que una entidad es quien dice ser
- Trazabilidad: Capacidad de rastrear las acciones de una entidad

## ISO 22989
Information technology and artificial intelligence: Este estándar proporciona un marco de referencia para la gestión de riesgos asociados con sistemas de inteligencia artificial, incluyendo aspectos de seguridad, privacidad y ética en el desarrollo y despliegue de soluciones de IA.

## ISO 27032
No es certificable porque es una "guía" de mejores prácticas, en comparación a la 27.001 (Sistema de Gestión de la Información) que tiene criterios específicos que pueden ser auditados. ISO 27032 se enfoca específicamente en la ciberseguridad y proporciona directrices para mejorar el estado de la seguridad en el ciberespacio.

## Fuentes

1. [Qué es la tríada CID](https://www.checkpoint.com/es/cyber-hub/cyber-security/what-is-it-security/what-is-the-cia-triad/)
2. [Riesgos en ciberseguridad](https://www.deltaprotect.com/blog/riesgos-de-ciberseguridad-ejemplos-y-prevencion)
3. [Vulnerabilidades INCIBE](https://www.incibe.es/incibe-cert/alerta-temprana/vulnerabilidades)
4. [Controles preventivos, detectivos y correctivos](https://www.auditool.org/blog/control-interno/cual-es-la-diferencia-entre-controles-preventivos-detectivos-y-correctivos)
5. [Marcos de ciberseguridad](https://preyproject.com/es/blog/marcos-de-ciberseguridad-la-guia-definitiva)