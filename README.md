<div align="center">
    <h2>«Gestión del desarrollo de sistemas de software de gran tamaño»</h2>
</div>

Este repositorio tiene como propósito contribuir a la preservación histórica y al análisis crítico de un artículo fundamental para la ingeniería de software: «Managing the Development of Large Software Systems», presentado por el Dr. Winston W. Royce en la IEEE WESCON en 1970. En él se establecen las bases del proceso de desarrollo de software, el cual, con el tiempo, ha sido interpretado —y en muchos casos simplificado— como el modelo «Waterfall».

---

## 1. Propósito del proyecto

El objetivo principal de este proyecto es doble:

- **Preservación histórica:** Publicar y conservar tres versiones del artículo:
  - La versión original (1970)
  - La versión digitalizada en inglés
  - La versión digitalizada traducida (inicialmente al español, con posibilidad de futuras traducciones)

- **Análisis crítico y reivindicación del legado del Dr. Royce:**
  - Presentar el análisis que realizó el Dr. Royce sobre el proceso de desarrollo de software secuencial, resaltando sus propuestas de mejora para mitigar los riesgos asociados a un proceso estrictamente lineal.
  - Corregir la interpretación errónea que llevó a popularizar el modelo «Waterfall», el cual ignoró los matices y las recomendaciones del Dr. Royce en cuanto a la iteración, el prototipado temprano y la consideración de limitaciones técnicas.
  - Discutir cómo las propuestas innovadoras del Dr. Royce anticiparon elementos que hoy se encuentran en las metodologías ágiles.

---

## 2. Introducción histórica y contexto

## 2.1. El origen del artículo

En agosto de 1970, durante la IEEE WESCON, el Dr. Royce presentó un artículo revolucionario basado en su experiencia en el desarrollo de software para misiones espaciales, donde la precisión y la confiabilidad eran esenciales. En su trabajo se abordaban:

- La planificación y el mando de misiones espaciales
- El análisis posterior al vuelo
- La gestión de sistemas complejos con recursos y restricciones severos (como «almacenamiento», «tiempo» y «procesamiento»)

## 2.2. Propósito original del artículo

El Dr. Royce no pretendía establecer un modelo definitivo de desarrollo de software; más bien, su intención era:

- Exponer los desafíos inherentes a los desarrollos a gran escala.
- Proponer mejoras al proceso secuencial tradicional, en el que la retroalimentación se daba demasiado tarde.
- Introducir conceptos como el prototipado temprano y la iteración, que anticiparían prácticas modernas en metodologías ágiles.

---

## 3. Proceso de desarrollo de software presentado por el Dr. Royce

## 3.1. Proceso de desarrollo simplificado

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022881/427214408-976bc1e4-b26b-4e3e-8c0f-c7657664065d_x5tcsc.png" height="250px">
</p>

El artículo original expone un modelo simplificado basado en dos pasos esenciales:

<ul>
  
## 3.1.1. Análisis (Analysis)
  - Comprensión de los requerimientos del sistema
  - Estudio de restricciones y limitaciones

## 3.1.2. Codificación (Coding)
  - Traducción de los requerimientos a código
  - Implementación de la funcionalidad

</ul>

> *Si bien este enfoque puede funcionar para proyectos pequeños, el Dr. Royce advirtió que, para sistemas de gran envergadura, resulta “condenado al fracaso” por la falta de flexibilidad y retroalimentación temprana.*

## 3.2. Proceso de desarrollo extendido

A continuación se describen brevemente las fases del proceso de desarrollo secuencial tal como las presentó el Dr. Winston W. Royce en su artículo *Managing the Development of Large Software Systems* (1970). Cada fase se concibe como un paso lógico que prepara el terreno para la siguiente, aunque Royce advierte que un flujo estrictamente lineal puede conllevar riesgos significativos si no se introducen mecanismos de retroalimentación y control.

<ul>

| Fase | Nombre | Propósito | Objetivos |
|------|--------|-----------|-------------|
| **1** | **Requerimientos del Sistema** | Establecer una comprensión clara y completa de las necesidades del sistema, incluyendo hardware, software y restricciones, para guiar el desarrollo en las fases posteriores. | Identificar y documentar los objetivos del sistema, las necesidades del usuario, las restricciones de alto nivel (como presupuesto, tiempo y tecnología), y los requisitos de hardware y software, sentando las bases para un desarrollo estructurado. |
| **2** | **Requerimientos de Software** | Definir con precisión los requisitos funcionales y no funcionales del software, asegurando que se alineen con los requerimientos del sistema y sean viables para la implementación. | Elaborar un documento detallado de requisitos de software (SRS) que incluya especificaciones funcionales, de rendimiento, seguridad y usabilidad; iterar con un diseño preliminar para validar la factibilidad técnica y operativa. |
| **3** | **Análisis** | Profundizar en los requisitos de software para identificar el alcance del problema, evaluar riesgos y planificar una solución técnica que cumpla con las expectativas del cliente. | Realizar un análisis exhaustivo de los requisitos para identificar inconsistencias, ambigüedades o conflictos; definir restricciones técnicas (como almacenamiento, tiempo de respuesta y capacidad); y establecer un plan inicial para el diseño, priorizando la viabilidad y la eficiencia. |
| **4** | **Diseño del Programa** | Crear una arquitectura detallada del software que sirva como un plano claro para la implementación, asegurando que el sistema sea modular, escalable y mantenible. | Diseñar la estructura del software, incluyendo módulos, interfaces, bases de datos y flujos de entrada/salida; asignar funciones específicas a cada componente; y documentar un diseño técnico detallado que sirva como guía para la codificación. |
| **5** | **Codificación** | Convertir el diseño técnico en código ejecutable, implementando el software de manera que cumpla con las especificaciones y mantenga la integridad del diseño planificado. | Escribir código limpio y eficiente siguiendo las especificaciones del diseño; realizar revisiones de código para garantizar adherencia a estándares de programación; y documentar el código para facilitar el mantenimiento futuro. |
| **6** | **Pruebas** | Validar que el software cumpla con todos los requisitos establecidos y funcione correctamente en todas las condiciones esperadas, identificando y corrigiendo defectos antes de la entrega. | Diseñar y ejecutar planes de prueba que incluyan pruebas unitarias, de integración, de sistema y de aceptación; emplear especialistas para inspeccionar errores; probar todas las rutas lógicas y condiciones de borde; y certificar que el software está listo para su despliegue. |
| **7** | **Operaciones** | Asegurar que el software opere de manera eficiente en el entorno de producción y se mantenga a lo largo del tiempo para satisfacer las necesidades cambiantes del usuario. | Desplegar el software en el entorno operativo; capacitar al personal de operaciones; monitorear el rendimiento del sistema; realizar mantenimiento correctivo, perfectivo y adaptativo; y documentar actualizaciones para garantizar la continuidad del sistema. |
<div align="center">
    <strong>Tabla: Fases del proceso de desarrollo extendido según el Dr. Royce<strong>
</div>
</br>

A continuación se presenta el diagrama original presentado en el artículo:

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022896/427214798-b711e803-99ea-4a16-86ff-9ed0010b4642_sh7jva.png">
</p>

## 3.2.1. Requerimientos del Sistema (System Requirements)

**Propósito:**  
Establecer el alcance global del proyecto y los objetivos generales del sistema que se pretende construir.

**Actividades clave:**  
- Identificación de las necesidades del cliente y las metas principales que el sistema debe cumplir.  
- Delimitación de los requisitos de alto nivel, incluyendo aspectos operativos y funcionales.  

## 3.2.2. Requerimientos de Software (Software Requirements)

**Propósito:**  
Traducir los requerimientos globales del sistema en especificaciones más detalladas y técnicas para el software.

**Actividades clave:**  
- Definición de las funcionalidades específicas que debe proporcionar el software.  
- Detalle de restricciones técnicas y operativas, incluyendo desempeño, compatibilidad, seguridad, etc.  

## 3.2.3. Análisis (Analysis)

**Propósito:**  
Comprender en profundidad el dominio del problema y estudiar en detalle cómo abordar las necesidades definidas en los requerimientos de software.

**Actividades clave:**  
- Identificación de estructuras de datos, flujos de información y lógicas de procesamiento.  
- Evaluación de posibles soluciones, considerando las restricciones identificadas en las fases anteriores.  

## 3.2.4. Diseño del Programa (Program Design)

**Propósito:**  
Definir la arquitectura del sistema, sus componentes internos y las interacciones entre ellos, antes de la implementación.

**Actividades clave:**  
- Estructuración de módulos y subsistemas, asignación de responsabilidades.  
- Diseño de interfaces, bases de datos y procedimientos de entrada/salida.  
- Planificación de recursos (almacenamiento, tiempo de ejecución, entre otros).  

## 3.2.5. Codificación (Coding)

**Propósito:**  
Implementar en software la solución diseñada, convirtiendo los requerimientos y diseños en un producto funcional.

**Actividades clave:**  
- Escritura y compilación de código siguiendo estándares de calidad.  
- Integración de módulos y subsistemas.  
- Revisión de código para asegurar consistencia y conformidad con el diseño.  

## 3.2.6. Pruebas (Testing)

**Propósito:**  
Verificar que el software cumpla con los requerimientos y que funcione correctamente en las condiciones previstas.

**Actividades clave:**  
- Ejecución de pruebas unitarias, de integración y de sistema.  
- Validación de cada ruta lógica para detectar errores o inconsistencias.  
- Análisis de desempeño y conformidad con las especificaciones iniciales.  

## 3.2.7. Operaciones (Operations)

**Propósito:**  
Desplegar el sistema en el entorno de producción y asegurar su funcionamiento continuo.

**Actividades clave:**  
- Puesta en marcha del software en la infraestructura del cliente.  
- Capacitación a los usuarios finales y equipos de soporte.  
- Monitoreo, mantenimiento y gestión de cambios posteriores a la entrega.  

</ul>

Estas fases se presentan de manera secuencial, pero el Dr. Royce enfatiza que, en la práctica, la retroalimentación y la iteración entre pasos son esenciales para reducir el riesgo de detectar errores o requerimientos cambiantes demasiado tarde. Por ello, él mismo propone una serie de mejoras —como la documentación exhaustiva, el prototipado temprano y la involucración del cliente— para complementar este flujo y hacerlo más adaptable y seguro.

## 3.3. Propuestas para mitigar los riesgos del proceso de desarrollo secuencial

Para evitar los problemas inherentes a un proceso estrictamente lineal (donde errores o cambios se detectan muy tarde), Royce sugiere cinco estrategias o "pasos" que se deben incorporar al proceso de desarrollo:

<ul>

## 3.3.1. Diseño del programa es lo primero:
Se propone iniciar el proceso con un diseño preliminar que se realice en el vacío de requisitos completos. Aunque este diseño pueda ser impreciso, sirve para identificar limitaciones técnicas (como las de almacenamiento, tiempo o procesamiento) de manera temprana, evitando que se incurra en errores costosos más adelante.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022913/427218390-466153c0-d29f-46e9-9cad-7b0b4dd37e1d_npd3sq.png">
</p>

## 3.3.2. Documentar el diseño:
Es fundamental elaborar una documentación exhaustiva que recoja todas las decisiones de diseño. Esto obliga a los equipos a comprometerse con una versión concreta del diseño y facilita la comunicación entre los distintos actores (diseñadores, analistas, clientes y gestores).

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022944/427218969-dbe7ea42-7541-4fac-a8c1-77021dc6e85a_uubozg.png">
</p>

## 3.3.3. Hazlo dos veces (realizar una simulación o prototipado piloto):
Royce recomienda ejecutar una versión preliminar o simulación del proceso de desarrollo. Este “ensayo” ayuda a detectar fallos críticos en un entorno controlado, permitiendo ajustar el diseño y los procesos antes de la implementación final.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022963/427219348-26a55ea0-be1b-44a2-973d-20d33fee7f94_mrfocw.png">
</p>

## 3.3.4. Planificar, controlar y supervisar las pruebas:
La fase de pruebas es la que más recursos consume y, en un proceso secuencial tradicional, es el primer punto donde se detectan errores significativos. Por ello, se debe gestionar rigurosamente esta etapa, asegurando que se verifiquen todas las rutas lógicas y se validen los aspectos operativos del sistema.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022979/427219588-163b7166-1611-4baa-a1e9-4ebee9eef728_bflepo.png">
</p>

## 3.3.5. Involucrar al cliente:
Se debe establecer un compromiso formal y continuo con el cliente en múltiples etapas del desarrollo. Esto permite obtener retroalimentación temprana y ajustar los requerimientos conforme avanza el proyecto, evitando discrepancias costosas en fases avanzadas.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022992/427219769-4679cbf2-5cb1-4899-8a05-c41e5ee1c368_y44epq.png">
</p>

</ul>

Estas propuestas buscan transformar un proceso de desarrollo arriesgado en uno que permita identificar, documentar y corregir errores de forma temprana, integrando iteraciones y validaciones que hoy son pilares de las metodologías ágiles.

---

## 4. Análisis crítico y reivindicación del legado del Dr. Royce

## 4.1. Interpretación errónea del modelo «Waterfall»

Aunque el análisis original del Dr. Royce contempla iteraciones y prototipado, con el tiempo se interpretó y simplificó su propuesta en un modelo secuencial rígido (el denominado «Waterfall»). Este malentendido ignoró:

- La importancia de la fase de retroalimentación temprana.
- La necesidad de ajustar continuamente los requerimientos y el diseño.
- Las recomendaciones del Dr. Royce para mitigar los riesgos inherentes a un proceso lineal.

## 4.2. Comparativa de enfoques

Existen dos visiones respecto al orden de las fases:

- **Enfoque del Dr. Royce:**
  - Iniciar con un prototipado temprano «en el vacío relativo de requisitos iniciales».
  - Permitir que el diseñador establezca restricciones operativas («almacenamiento», «tiempo», «procesamiento») que luego guíen el análisis.

- **Enfoque alternativo (actual):**
  - Realizar un análisis completo de requerimientos antes de proceder con el prototipado.
  - Posteriormente, utilizar el prototipo para validar y ajustar los requerimientos ya definidos.

> *Si bien en 1970 las limitaciones técnicas justificaban el enfoque de Royce, en 2025, con recursos computacionales prácticamente ilimitados, resulta factible y, en teoría, más eficiente comenzar con un análisis detallado que minimice la incertidumbre inicial. No obstante, la necesidad de iterar y validar mediante prototipos continúa siendo relevante, por lo que la integración de ambos enfoques —un análisis exhaustivo seguido de un prototipado iterativo— puede representar la mejor práctica actual.*

---

## 5. Análisis y visión actualizada (2025)

En el contexto actual, los avances en ingeniería de software y el surgimiento de metodologías ágiles permiten:

- **Un análisis de requerimientos más robusto:**  
  La madurez tecnológica y la disponibilidad de recursos facilitan la recopilación y el análisis exhaustivo de requerimientos, reduciendo la variabilidad entre fases.

- **Iteración constante:**  
  Aunque el análisis inicial puede ser más completo, la validación y el ajuste mediante prototipos siguen siendo fundamentales para adaptarse a cambios o nuevos requerimientos durante el desarrollo.

- **Fusión de enfoques:**  
  La tendencia actual es integrar lo mejor de ambos mundos: un análisis profundo que establezca una base sólida y un prototipado iterativo que permita validar y ajustar el diseño en tiempo real.

> *Esta visión actualizada permite no solo reconocer la relevancia histórica del Dr. Royce, sino también reinterpretar sus propuestas en un marco moderno, donde se revalorizan tanto la precisión del análisis como la flexibilidad y adaptabilidad del prototipado.*

---

## 6. Documentos incluidos en el repositorio

Este repositorio contiene tres versiones del artículo:

- **Versión original (1970):**  
  El documento escaneado tal como fue presentado en la IEEE WESCON.
- **Versión digitalizada (inglés):**  
  Una versión digital que preserva el formato y el contenido original.
- **Versión digitalizada traducida (español):**  
  Una traducción inicial al español, con posibilidad de futuras traducciones a otros idiomas.

---

## 7. Conclusión

Este proyecto busca honrar y reinterpretar el trabajo del Dr. Royce, demostrando que sus propuestas van más allá de un simple modelo secuencial. Su visión integradora y su enfoque en la mitigación de riesgos a través del prototipado y la iteración anticipada sentaron las bases para lo que hoy conocemos como metodologías ágiles. La evolución del desarrollo de software, tanto en teoría como en práctica, nos invita a fusionar lo mejor de ambos enfoques para lograr procesos más eficientes y adaptables en el contexto actual.

Esperamos que este repositorio sirva de referencia tanto para historiadores de la ingeniería de software como para profesionales que buscan comprender la evolución de los procesos de desarrollo y las raíces de las prácticas ágiles actuales.

---

*Este README puede ser adaptado y ampliado conforme surja nueva información o se deseen incorporar nuevos análisis y traducciones. ¡Bienvenido a «SoftwareDevelopment-Lifecycle»!*
