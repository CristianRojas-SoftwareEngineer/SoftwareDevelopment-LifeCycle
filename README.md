
<div align="center">
  <h1>» Artículo en construcción «</h1>
</div>

---

<div align="center">
    <h2>Rediseño del ciclo de vida del software a gran escala</h2>
</div>

## Introducción

El artículo titulado **«Managing the development of large software systems»** fue presentado por el Dr. Winston Walker Royce (1929 – 1995) en la 26ª edición de la convención WESCON (*Western Electronic Show and Convention*), realizada en agosto de 1970. Esta convención era organizada anualmente por el IEEE (*Institute of Electrical and Electronics Engineers*), con el propósito de ofrecer un espacio colaborativo para la presentación y discusión de avances tecnológicos y científicos en los campos de la electrónica y la ingeniería.

Fue en este espacio donde el Dr. Royce presentó uno de los primeros modelos de proceso de desarrollo de sistemas de software reconocidos, y por lo tanto, fundamentales en el ámbito de la ingeniería de software, el cual, posteriormente, sería interpretado y definido —aunque de manera incompleta— como el «*waterfall process model*», o «*modelo de proceso en cascada*», de acuerdo con su traducción al español. Sin embargo, el artículo presentado no se limitó a describir un modelo de proceso de desarrollo estructurado en fases, sino que también presentó un análisis sobre los riesgos potenciales de implementar un proceso de desarrollo estrictamente secuencial.

Según Royce, aunque abordar el proceso de desarrollo de software siguiendo un enfoque secuencial es válido, "es arriesgado e invita al fracaso", ya que la validación del proyecto, que abarca tanto la definición y el análisis de los requerimientos como el diseño y la codificación del software, ocurre de forma tardía, durante la fase de pruebas, al final del ciclo de desarrollo. Esta retroalimentación tardía es riesgosa, ya que si durante la fase de pruebas se detecta que el software no cumple ya sea con los requerimientos funcionales o bien con las restricciones de integración con el entorno operativo, podría ser necesario modificar el diseño del software o incluso redefinir los requerimientos del mismo, lo que puede ocasionar retrasos significativos en la planificación del proyecto e incluso causar un sobrecosto de hasta el 100%, tanto en plazos como en inversión económica.

Finalmente, luego de analizar el modelo de proceso de desarrollo de software presentado, y tras reconocer los riesgos inherentes al proceso de desarrollo secuencial, el Dr. Royce propuso cinco prácticas clave para refinar el proceso de desarrollo de software, mejorar la calidad del software producido y asegurar una mayor alineación entre las necesidades de los usuarios y las funcionalidades implementadas en el sistema desarrollado.

Algunas de estas prácticas establecieron las bases para el paradigma ágil de desarrollo de software, tales como el enfoque iterativo, el desarrollo basado en prototipos, la retroalimentación temprana y el involucramiento del cliente como parte fundamental del equipo de desarrollo.

---

## Propósito de este proyecto

El propósito de este proyecto es contribuir a la preservación histórica del artículo *«Managing the development of large software systems»*, el cual es considerado un aporte fundamental para la ingeniería de software.

Este repositorio contiene tres versiones del artículo:
  - **Versión original (1970):**  
    Artículo original escaneado, publicado en la 26ª edición de la convención WESCON, realizada en 1970.
  - **Versión digitalizada (inglés):**  
    Una versión digital que preserva el formato y el contenido original.
  - **Versión digitalizada traducida (español):**  
    Una traducción inicial al español, con posibilidad de futuras traducciones a otros idiomas.

**Análisis crítico y reivindicación del legado del Dr. Royce:**
  - Presentar el análisis que realizó el Dr. Royce sobre el proceso de desarrollo de software secuencial, resaltando sus propuestas de mejora para mitigar los riesgos asociados a un proceso estrictamente lineal.
  - Corregir la interpretación errónea que llevó a popularizar el modelo «Waterfall», el cual ignoró los matices y las recomendaciones del Dr. Royce en cuanto a la iteración, el prototipado temprano y la consideración de limitaciones técnicas.
  - Discutir cómo las propuestas innovadoras del Dr. Royce anticiparon elementos que hoy se encuentran en las metodologías ágiles.

---

## Índice del artículo

A continuación se presenta el índice del artículo para facilitar la navegación por el mismo. El artículo se encuentra estructurado de la siguiente manera:

[**» 1. Contexto histórico del artículo original**](#1-contexto-sobre-el-artículo-original)</br>
[**» 2. Proceso de desarrollo de software presentado por el Dr. Royce**](#2-proceso-de-desarrollo-de-software-presentado-por-el-dr-royce)</br>
[**» 3. Mejoras propuestas por el Dr. Royce**](#3-propuestas-de-mejora-para-el-proceso-de-desarrollo-de-software-sugeridas-por-el-dr-royce)</br>
[**» 4. ¿Por qué el «modelo en cascada» del ciclo de vida del software es una interpretación incompleta?**](#4-por-qué-el-modelo-de-proceso-en-cascada-es-una-interpretación-incompleta)</br>
[**» 5. Mi interpretación del artículo original**](#5-mi-análisis-sobre-el-proceso-de-desarrollo-de-software-presentado)</br>
[**» 6. Mi propuesta de modelo de ciclo de vida del software**](#6-conclusiones)</br>
[**» 7. Conclusiones**](#6-conclusiones)</br>

Puedes navegar directamente a cada sección del artículo presionando sobre su respectivo título.

---

## 1. Contexto sobre el artículo original

dada su experiencia en la gestión y desarrollo de proyectos de ingeniería aeroespacial, el Dr. Royce

reducir el riesgo de necesitar aplicar modificaciones disruptivas en fases avanzadas del proceso de desarrollo

## 1.1. El origen del artículo

En agosto de 1970, durante la IEEE WESCON, el Dr. Royce presentó un artículo revolucionario basado en su experiencia en el desarrollo de software para misiones espaciales, donde la precisión y la confiabilidad eran esenciales. En su trabajo se abordaban:

- La planificación y el mando de misiones espaciales
- El análisis posterior al vuelo
- La gestión de sistemas complejos con recursos y restricciones severos (como «almacenamiento», «tiempo» y «procesamiento»)

## 1.2. Propósito original del artículo

El Dr. Royce no pretendía establecer un modelo definitivo de desarrollo de software; más bien, su intención era:

- Exponer los desafíos inherentes a los desarrollos a gran escala.
- Proponer mejoras al proceso secuencial tradicional, en el que la retroalimentación se daba demasiado tarde.
- Introducir conceptos como el prototipado temprano y la iteración, que anticiparían prácticas modernas en metodologías ágiles.

---

## 2. Proceso de desarrollo de software presentado por el Dr. Royce

## 2.1. Proceso de desarrollo simplificado

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022881/427214408-976bc1e4-b26b-4e3e-8c0f-c7657664065d_x5tcsc.png" height="250px">
</p>

El artículo original expone un modelo simplificado basado en dos pasos esenciales:

<ul>
  
## 2.1.1. Análisis (Analysis)
  - Comprensión de los requerimientos del sistema
  - Estudio de restricciones y limitaciones

## 2.1.2. Codificación (Coding)
  - Traducción de los requerimientos a código
  - Implementación de la funcionalidad

</ul>

> *Si bien este enfoque puede funcionar para proyectos pequeños, el Dr. Royce advirtió que, para sistemas de gran envergadura, resulta “condenado al fracaso” por la falta de flexibilidad y retroalimentación temprana.*

## 2.2. Proceso de desarrollo extendido

En su artículo de 1970, el Dr. Royce describió un enfoque más estructurado para el desarrollo de software que el simple modelo de dos pasos de análisis y codificación. Este enfoque inicial se desglosaba en siete fases secuenciales para el desarrollo de grandes sistemas de software:
1. Requerimientos del Sistema.
2. Requerimientos de Software.
3. Análisis.
4. Diseño del Programa.
5. Codificación.
6. Pruebas.
7. Operaciones.

Es fundamental comprender que Royce presentó este modelo como un punto de partida para ilustrar la necesidad de definir un proceso de desarrollo integral, antes de discutir las mejoras y la naturaleza iterativa que consideraba esencial. A continuación se presenta una tabla en dónde se sintetizan el propósito y objetivos concretos de cada fase, considerando desde la definición y análisis de requerimientos en las fases iniciales, hasta la puesta en marcha, capacitación de usuarios, monitoreo y mantenimiento contínuo durante las fases finales del proceso de desarrollo y producción de sistemas de software de gran tamaño:

| Fase | Nombre | Propósito | Objetivos |
|------|--------|-----------|-------------|
| **1** | **Requerimientos del Sistema** | Establecer una comprensión de alto nivel de las necesidades generales del proyecto, incluyendo metas, expectativas del cliente y restricciones. | <strong>»</strong> Identificación de las necesidades del cliente y las metas principales que el sistema debe cumplir.</br><strong>»</strong> Delimitación de los requisitos de alto nivel, incluyendo aspectos operativos y funcionales. |
| **2** | **Requerimientos de Software** | Traducir los requerimientos del sistema en especificaciones detalladas y precisas para el software que se va a desarrollar. | <strong>»</strong> Definición de las funcionalidades específicas que debe proporcionar el software.</br><strong>»</strong> Detalle de restricciones técnicas y operativas, incluyendo desempeño, compatibilidad, seguridad, etc. |
| **3** | **Análisis** | Estudiar el problema en profundidad y concebir una estrategia técnica general para su resolución mediante software. | <strong>»</strong> Identificación de estructuras de datos, flujos de información y lógicas de procesamiento.</br><strong>»</strong> Evaluación de posibles soluciones, considerando las restricciones identificadas en las fases anteriores. |
| **4** | **Diseño del Programa** | Crear un diseño detallado de la arquitectura del software, incluyendo componentes, módulos, interfaces y su interacción. | <strong>»</strong> Estructuración de módulos y subsistemas, asignación de responsabilidades.</br><strong>»</strong> Diseño de interfaces, bases de datos y procedimientos de entrada/salida.</br><strong>»</strong> Planificación de recursos (almacenamiento, tiempo de ejecución, entre otros). |
| **5** | **Codificación** | Implementar el diseño del software en código fuente ejecutable en un lenguaje de programación específico. | <strong>»</strong> Escritura y compilación de código siguiendo estándares de calidad.</br><strong>»</strong> Integración de módulos y subsistemas.</br><strong>»</strong> Revisión de código para asegurar consistencia y conformidad con el diseño. |
| **6** | **Pruebas** | Verificar y validar que el software cumple con los requisitos y funciona correctamente en diversas condiciones. | <strong>»</strong> Ejecución de pruebas unitarias, de integración y de sistema.</br><strong>»</strong> Validación de cada ruta lógica para detectar errores o inconsistencias.</br><strong>»</strong> Análisis de desempeño y conformidad con las especificaciones iniciales. |
| **7** | **Operaciones** | Desplegar y mantener el software en el entorno de producción para asegurar su funcionamiento continuo y satisfacer las necesidades del usuario. | <strong>»</strong> Puesta en marcha del software en la infraestructura del cliente.</br><strong>»</strong> Capacitación a los usuarios finales y equipos de soporte.</br><strong>»</strong> Monitoreo, mantenimiento y gestión de cambios posteriores a la entrega. |
<div align="center">
    <strong>Tabla: Fases del proceso de desarrollo extendido según el Dr. Royce</strong>
</div>
</br>

A continuación se presenta el diagrama original presentado en el artículo:

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022896/427214798-b711e803-99ea-4a16-86ff-9ed0010b4642_sh7jva.png">
</p>

Estas fases se presentan de manera secuencial, pero el Dr. Royce enfatiza que, en la práctica, la retroalimentación y la iteración entre pasos son esenciales para reducir el riesgo de detectar errores o requerimientos cambiantes demasiado tarde. Por ello, él mismo propone una serie de mejoras —como la documentación exhaustiva, el prototipado temprano y la involucración del cliente— para complementar este flujo y hacerlo más adaptable y seguro.

---

## 3. Propuestas de mejora para el proceso de desarrollo de software sugeridas por el Dr. Royce

Para evitar los problemas inherentes a un proceso estrictamente lineal (donde errores o cambios se detectan muy tarde), Royce sugiere cinco estrategias o "pasos" que se deben incorporar al proceso de desarrollo:

<ul>

## 3.1. Diseño del programa es lo primero:
Se propone iniciar el proceso con un diseño preliminar que se realice en el vacío de requisitos completos. Aunque este diseño pueda ser impreciso, sirve para identificar limitaciones técnicas (como las de almacenamiento, tiempo o procesamiento) de manera temprana, evitando que se incurra en errores costosos más adelante.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022913/427218390-466153c0-d29f-46e9-9cad-7b0b4dd37e1d_npd3sq.png">
</p>

## 3.2. Documentar el diseño:
Es fundamental elaborar una documentación exhaustiva que recoja todas las decisiones de diseño. Esto obliga a los equipos a comprometerse con una versión concreta del diseño y facilita la comunicación entre los distintos actores (diseñadores, analistas, clientes y gestores).

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022944/427218969-dbe7ea42-7541-4fac-a8c1-77021dc6e85a_uubozg.png">
</p>

## 3.3. Hazlo dos veces (realizar una simulación o prototipado piloto):
Royce recomienda ejecutar una versión preliminar o simulación del proceso de desarrollo. Este “ensayo” ayuda a detectar fallos críticos en un entorno controlado, permitiendo ajustar el diseño y los procesos antes de la implementación final.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022963/427219348-26a55ea0-be1b-44a2-973d-20d33fee7f94_mrfocw.png">
</p>

## 3.4. Planificar, controlar y supervisar las pruebas:
La fase de pruebas es la que más recursos consume y, en un proceso secuencial tradicional, es el primer punto donde se detectan errores significativos. Por ello, se debe gestionar rigurosamente esta etapa, asegurando que se verifiquen todas las rutas lógicas y se validen los aspectos operativos del sistema.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022979/427219588-163b7166-1611-4baa-a1e9-4ebee9eef728_bflepo.png">
</p>

## 3.5. Involucrar al cliente:
Se debe establecer un compromiso formal y continuo con el cliente en múltiples etapas del desarrollo. Esto permite obtener retroalimentación temprana y ajustar los requerimientos conforme avanza el proyecto, evitando discrepancias costosas en fases avanzadas.

<p align="center">
  <img src="https://res.cloudinary.com/dqdvzzemd/image/upload/v1743022992/427219769-4679cbf2-5cb1-4899-8a05-c41e5ee1c368_y44epq.png">
</p>

</ul>

Estas propuestas buscan transformar un proceso de desarrollo arriesgado en uno que permita identificar, documentar y corregir errores de forma temprana, integrando iteraciones y validaciones que hoy son pilares de las metodologías ágiles.

---

## 4. ¿Por qué el «modelo de proceso en cascada» es una interpretación incompleta?

[Interpretación errónea del modelo «Waterfall»]
Aunque el análisis original del Dr. Royce contempla iteraciones y prototipado, con el tiempo se interpretó y simplificó su propuesta en un modelo secuencial rígido (el denominado «Waterfall»). Este malentendido ignoró:

- La importancia de la fase de retroalimentación temprana.
- La necesidad de ajustar continuamente los requerimientos y el diseño.
- Las recomendaciones del Dr. Royce para mitigar los riesgos inherentes a un proceso lineal.

---

## 5. Mi interpretación del modelo de proceso de desarrollo de software presentado

En el contexto actual, los avances en ingeniería de software y el surgimiento de metodologías ágiles permiten:

- **Un análisis de requerimientos más robusto:**  
  La madurez tecnológica y la disponibilidad de recursos facilitan la recopilación y el análisis exhaustivo de requerimientos, reduciendo la variabilidad entre fases.

- **Iteración constante:**  
  Aunque el análisis inicial puede ser más completo, la validación y el ajuste mediante prototipos siguen siendo fundamentales para adaptarse a cambios o nuevos requerimientos durante el desarrollo.

- **Fusión de enfoques:**  
  La tendencia actual es integrar lo mejor de ambos mundos: un análisis profundo que establezca una base sólida y un prototipado iterativo que permita validar y ajustar el diseño en tiempo real.

> *Esta visión actualizada permite no solo reconocer la relevancia histórica del Dr. Royce, sino también reinterpretar sus propuestas en un marco moderno, donde se revalorizan tanto la precisión del análisis como la flexibilidad y adaptabilidad del prototipado.*

Existen dos visiones respecto al orden de las fases:

- **Enfoque del Dr. Royce:**
  - Iniciar con un prototipado temprano «en el vacío relativo de requisitos iniciales».
  - Permitir que el diseñador establezca restricciones operativas («almacenamiento», «tiempo», «procesamiento») que luego guíen el análisis.

- **Enfoque alternativo (actual):**
  - Realizar un análisis completo de requerimientos antes de proceder con el prototipado.
  - Posteriormente, utilizar el prototipo para validar y ajustar los requerimientos ya definidos.

> *Si bien en 1970 las limitaciones técnicas justificaban el enfoque de Royce, en 2025, con recursos computacionales prácticamente ilimitados, resulta factible y, en teoría, más eficiente comenzar con un análisis detallado que minimice la incertidumbre inicial. No obstante, la necesidad de iterar y validar mediante prototipos continúa siendo relevante, por lo que la integración de ambos enfoques —un análisis exhaustivo seguido de un prototipado iterativo— puede representar la mejor práctica actual.*

---

## 6. Mi propuesta de modelo de ciclo de vida del software

En el contexto actual, los avances en ingeniería de software y el surgimiento de metodologías ágiles permiten:

- **Un análisis de requerimientos más robusto:**  
  La madurez tecnológica y la disponibilidad de recursos facilitan la recopilación y el análisis exhaustivo de requerimientos, reduciendo la variabilidad entre fases.

- **Iteración constante:**  
  Aunque el análisis inicial puede ser más completo, la validación y el ajuste mediante prototipos siguen siendo fundamentales para adaptarse a cambios o nuevos requerimientos durante el desarrollo.

- **Fusión de enfoques:**  
  La tendencia actual es integrar lo mejor de ambos mundos: un análisis profundo que establezca una base sólida y un prototipado iterativo que permita validar y ajustar el diseño en tiempo real.

> *Esta visión actualizada permite no solo reconocer la relevancia histórica del Dr. Royce, sino también reinterpretar sus propuestas en un marco moderno, donde se revalorizan tanto la precisión del análisis como la flexibilidad y adaptabilidad del prototipado.*

Existen dos visiones respecto al orden de las fases:

- **Enfoque del Dr. Royce:**
  - Iniciar con un prototipado temprano «en el vacío relativo de requisitos iniciales».
  - Permitir que el diseñador establezca restricciones operativas («almacenamiento», «tiempo», «procesamiento») que luego guíen el análisis.

- **Enfoque alternativo (actual):**
  - Realizar un análisis completo de requerimientos antes de proceder con el prototipado.
  - Posteriormente, utilizar el prototipo para validar y ajustar los requerimientos ya definidos.

> *Si bien en 1970 las limitaciones técnicas justificaban el enfoque de Royce, en 2025, con recursos computacionales prácticamente ilimitados, resulta factible y, en teoría, más eficiente comenzar con un análisis detallado que minimice la incertidumbre inicial. No obstante, la necesidad de iterar y validar mediante prototipos continúa siendo relevante, por lo que la integración de ambos enfoques —un análisis exhaustivo seguido de un prototipado iterativo— puede representar la mejor práctica actual.*

---

## 7. Conclusiones

El artículo **«Managing the development of large software systems»** presentado por el Dr. Royce en la 26ª edición de la convención WESCON realizada en agosto de 1970, es fundamental para la ingeniería de software, ya que en él se presentó uno de los primeros enfoques estructurados para la gestión del proceso de desarrollo de software, en un momento en que la industria comenzaba a enfrentar grandes dificultades para desarrollar sistemas cada vez más complejos.

Además, es importante destacar que el aporte realizado por el Dr. Royce no se limita a la definición del «*modelo de proceso en cascada*» —atribuido erróneamente—, ya que algunas de las prácticas sugeridas por Royce establecieron las bases para el paradigma de desarrollo ágil de software, consolidado más de 30 años después de esta publicación, tras la creación del «Manifiesto Ágil» en el año 2001, definido y validado por 17 expertos en desarrollo de software de la época.

Es importante destacar la profunda comprensión sobre el proceso de desarrollo de software demostrada por el Dr. Royce,

Este proyecto busca honrar y reinterpretar el trabajo del Dr. Royce, demostrando que sus propuestas van más allá de un simple modelo secuencial. Su visión integradora y su enfoque en la mitigación de riesgos a través del prototipado y la iteración anticipada sentaron las bases para lo que hoy conocemos como metodologías ágiles. La evolución del desarrollo de software, tanto en teoría como en práctica, nos invita a fusionar lo mejor de ambos enfoques para lograr procesos más eficientes y adaptables en el contexto actual.

Esperamos que este repositorio sirva de referencia tanto para historiadores de la ingeniería de software como para profesionales que buscan comprender la evolución de los procesos de desarrollo y las raíces de las prácticas ágiles actuales.

---

## Acerca de este repositorio

- Los documentos contenidos en este repositorio están sujetos a modificación en caso de detectarse errores en la redacción, digitalización o traducción del artículo  **«Managing the development of large software systems»**.

- Además, con el propósito de extender el alcance del artículo presentado por el Dr. Royce, este repositorio podría ser actualizado para incluir nuevas traducciones a otros idiomas.

---

## Autor

**Cristian Rojas Arredondo**  
Ingeniero de Software | Licenciado en Ingeniería Informática, Universidad de Valparaíso, Chile
Contacto: cristian.rojas.software.engineer@gmail.com

## Licencia y distribución

Copyright © 2025 Cristian Rojas Arredondo

Este proyecto se distribuye bajo los términos de la «Creative Commons Zero 1.0 Universal (CC0 1.0)», lo que significa que el autor renuncia a todos los derechos de autor y de propiedad intelectual en la medida permitida por la ley, dedicando el contenido al dominio público.

## Libertades otorgadas

La licencia «Creative Commons Zero» permite a cualquier persona:

- **Copiar, modificar y redistribuir** el contenido sin restricciones, ya sea de forma gratuita o comercial.
- **Utilizar el contenido** para cualquier propósito, sin necesidad de atribución obligatoria.
- **Crear obras derivadas** basadas en este contenido sin limitación alguna.

## Recomendaciones

Bajo la licencia «Creative Commons Zero» no se imponen condiciones legales; sin embargo, se recomienda tener en cuenta lo siguiente:

- **Reconocimiento:** Al distribuir el contenido de este repositorio o cualquier obra derivada de él, se sugiere mencionar que este repositorio es la fuente original, como muestra de cortesía. Además, esta mención ayudará tanto a la preservación histórica del artículo original como a la divulgación completa del análisis sobre el proceso de desarrollo de software presentado por el Dr. Royce en dicho artículo.
- **Uso responsable:** Si bien cualquier persona puede utilizar el contenido de este repositorio para cualquier propósito, se insta a utilizar dicho contenido de forma responsable y ética, procurando que su uso contribuya positivamente a la comunidad académica y profesional.

## Documentación legal

La versión completa y legalmente vinculante de la licencia «Creative Commons Zero 1.0 Universal» se encuentra en el archivo [LICENSE](LICENSE) ubicado en la raíz del proyecto. Este documento contiene el texto oficial de la licencia, el cual es el único con validez legal.

*Nota: Al utilizar, modificar o redistribuir este contenido, se entiende que lo haces de acuerdo con los términos de la licencia. Se recomienda revisar el archivo LICENSE para comprender plenamente los derechos y condiciones aplicables.*

---

<div align="center">
  <h1>» Artículo en construcción «</h1>
</div>
