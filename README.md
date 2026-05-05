Proyecto realizado en el margen de fechas: 19/09/2024 - 23/01/2025

[GitHub: Ch4mbi](https://github.com/Ch4mbi)


**Índice**

Contenido

Análisis Forense y respuesta ante incidentes

Fases de proceso de análisis forense

Análisis Forense Digital

Ventajas y desventajas

Directrices de las fuerzas de seguridad

Ético

Investigación Forense Digital	

Planificación

Comparación de herramientas	

Funcionamiento del sistema operativo

HashMyFiles	

Narcos 1	

Primeras Imágenes de drogas	

Mapas	

Billete	

Búsqueda de drogas	

Historial

Narcos 2

Billete	

Excel de clientes

Programa de ocultación de secretos	

Imagen de localización de drogas	

Posibles métodos de ocultación de drogas

Imágenes de calle

Contact Card

Narcos 3	

Imagen de grabación	

Búsquedas de internet sospechosas	

[\#\# Herramienta sospechosa en descargas	

Quasar.v.1.3.0.0	

BNE	

Intento de descifrar secreto	

Método de comunicación alternativo	

Conclusión	

TEST PLAN	

Pasos para Test plan eficiente	

Poner los pasos en práctica	

Diagrama	

Buenas prácticas	

Prácticas para toda investigación	

Prácticas para este caso específico	

Evaluación crítica personal	

Bibliografía	
 
 
[GitHub: Ch4mbi](https://github.com/Ch4mbi)


# Análisis Forense y respuesta ante incidentes {##-análisis-forense-y-respuesta-ante-incidentes}

El puesto de forense digital es una de las diversas ramas que forman parte de la ciberseguridad. Los que trabajan en este ámbito se dedican a la investigación tras un ataque o investigar crímenes en los que haya involucrado algún dispositivo electrónico (Móvil, PC, etc). A pesar de que sea una rama de la ciberseguridad, más bien se centra en analizar los equipos tras un ataque o crimen. Los que se encargan de mitigar el ataque y de eliminarlo o de reducir su impacto final están más enfocados a la respuesta ante incidentes en tiempo real mientras que los forenses digitales se dedican a analizarlo tras que haya sucedido. Se dedican a recuperar equipos, archivos, hardware, etc., y a analizarlos y a realizar informes de los afectados para un uso posterior.  Lo cual  puede ser de utilidad en diversas situaciones judiciales ,por ejemplo, en la obtención de evidencias clave en un delito digital(Evidencia digital). Los forenses digitales se centran en descubrir:

- **Qué ha pasado**:  
  Se centra en analizar el equipo afectado con el fin de descubrir lo que ha pasado.

- **Cuales son los efectos que ha tenido el ataque sobre los dispositivos afectados**:  
  	Esto se debe a que el puesto de forense digital no solo analiza hardware criminal, sino que también analiza, por ejemplo, un servidor que ha sido atacado para saber como se ha llevado a cabo un ciberataque en ese servidor y que se puedan obtener soluciones para que no se vuelva a repetir dicho ataque, o también para saber qué ha pasado con exactitud e intentar recuperar archivos que hayan sido eliminados en el ataque o directamente eliminados por el criminal.

- **Sobre qué dispositivos se ha llevado a cabo el ataque**  
  	Ya sean dispositivos móviles, portátiles, ordenadores personales, discos duros o servidores. Es importante conocer sobre qué dispositivo se va a trabajar para poder seguir un procedimiento adecuado (y sobre el sistema operativo del mismo).

- **Como se ha llevado a cabo ese ataque:**  
  	Este punto se centra en analizar qué y cómo se ha producido un ataque y poder analizar archivos que hayan sido alterados o eliminados. Esto permite a los forenses digitales reconstruir cómo fue el ataque, y lo que sucedió después y antes del mismo. 

- **Autoría:**  
  	Localizar al autor de dicho ataque (U obtener una dirección IP, una red, una identidad, etc). 

Los analistas forenses son defensivos, no ofensivos. Hay que tener en cuenta también que los analistas de un SOC también son forenses.

Mientras que los que se centran en la respuesta ante incidentes se centran en:

- **Contener o evitar** un ataque informático.  
- **Evitar la propagación** del mismo.  
- **Implementar medidas preventivas** una vez eliminado para evitar ataques similares.

Estos conocimientos del ataque ayudan a conocer la naturaleza de un ataque informático en uno o varios dispositivos y, así, poder proveerlos o hallar al autor/es de dicho ataque, o recuperar archivos eliminados o alterados de un dispositivo atacado. Aunque también puede ser útil para ayudar a organizaciones a prevenir nuevos ataques similares (Dependiendo del contexto en el que el forense digital trabaje). Esto estará más relacionado con la respuesta ante incidentes:

- Analizar un incidente (Ataque, o intento del mismo, robo de información, etc).  
- Evitar la propagación del ataque en tiempo real o a futuro por si se repite.  
- Neutralizar el ataque o el programa malicioso.  
- Restaurar servicios (Si es un servidor de una empresa, por ejemplo) o el equipo afectado.

Estos puntos tienen similitudes con la respuesta ante incidentes debido a que ambos deben prever futuros ataques y establecer medidas preventivas (Siempre bajo el contexto adecuado). Los forenses digitales llevan a cabo una serie de fases o procedimientos a la hora de ponerse a trabajar en un análisis forense de un dispositivo. 

## Fases de proceso de análisis forense {###-fases-de-proceso-de-análisis-forense}

Visto a simple vista, el proceso de análisis que lleva a cabo un forense digital suele tener los mismos pasos en todas las situaciones. Se puede decir que es hasta un proceso repetitivo, pero cuando se profundiza en cada paso, se entiende que cada paso es más profundo de lo que aparenta. Esto es una metodología básica que se debe seguir, pudiéndose alterar si la situación lo requiere

1. **Desarrollo de políticas**:   
   	Establecer una serie de regulaciones, pasos y procedimientos para comenzar a analizar los dispositivos. Se deben establecer objetivos claros y saber y tener claro como encontrar o recuperar lo que estamos buscando. También hay que pensar en cómo podemos proceder de manera segura sin dañar o alterar el equipo afectado.

2. **Evaluación e identificación de evidencias**:  
   	Se clasifican las evidencias en base a su prioridad, para tener un orden de relevancia en las mismas (Archivos, USBs, Discos duros, imágenes, etc).

3. **Adquisición de evidencias** (**Cadena de custodia**):  
   	Preservando el documentado todo el proceso. Se debe emplear siempre medios contra escritura en la evidencia digital y tener en cuenta los medios de almacenamiento más volátiles. Se pueden obtener los logs de los sistemas operativos, analizar los nombres de los archivos o los propios archivos en sí, contraseñas, inicios de sesión, el historial, etc.

4. **Análisis**:  
   	Analizar el dispositivo en busca de cambios, conocer los efectos y posible alcance del incidente. Se analizan las evidencias para obtener conclusiones. Se usan herramientas especializadas en recuperar archivos, o en buscar los mismos. 

5. **Documentación y reporting**:  
   	En este paso se deben hacer 2 reportes:  
   * Uno explicando lo que ha pasado sin entrar en detalles, con una visión más general del caso  
   * Otro especificando qué pasos se han llevado a cabo con exactitud. Este se debe hacer a la par que se está analizando el equipo para garantizar la precisión de los pasos llevados a cabo.

(Martinez, s.f.)  
El hecho de seguir una serie de pasos, o una metodología predefinida, para recuperar información o analizar un equipo es muy importante, ya que el no seguirla dificulta la adquisición de evidencias, y no es solo para nosotros, ya que, si sabemos lo que hacemos, se pueden sacar conclusiones, sino para la gente para la que estamos llevando a cabo el análisis forense, con esto me refiero a que se puede perder la veracidad de los datos. Por ejemplo:

- En una investigación de un crimen, debemos hacer un reporte si no se sigue una metodología predefinida, a la hora de presentar el reporte será confuso. En el reporte se deben poner imágenes, que hay que tener en cuenta que no bastan como evidencia, sino como” guía”, se deben poner las rutas o pasos específicos para que los que lean el reporte puedan llegar hasta donde nosotros hemos llegado y ver la evidencia(Eso en la parte de reporing y análisis, ya que se deben hacer a la vez o llevará a perdidas de los procedimientos). Si los que leen el reporte, por ejemplo en un juicio, no son capaces de saber dónde se ha encontrado la evidencia, se anularía lo que hemos encontrado aunque le hayamos tomado fotos.  
- Otro aspecto de la metodología es el desarrollo de políticas, es necesario cumplir con este paso, si no se analizan las políticas de privacidad antes, podemos llegar a estar involucrados en otro crimen u otros problemas legales.  
- También se deben identificar las evidencias antes de analizar el dispositivo, si no, se puede alargar el tiempo de búsqueda y llevar a cabo un análisis peor.

Desde mi punto de vista, seguir una metodología definida antes de comenzar el proceso de investigación es la mejor opción por la que podemos optar, ya que nos quitamos preocupaciones que tendríamos si seguimos con la investigación sin metodología (como los problemas legales o el hecho de hacer entender a la gente que lee el informe lo que están vendo y como pueden llegar a esos puntos). A demás, a mi parecer, se logra un informe mejor estructurado y un análisis bien llevado a cabo si se siguen unos pasos predefinidos, una buena idea es usar un diagrama para saber que hacer a continuación y no perder tiempo en decidir qué hacer.   
A la hora de analizar un equipo atacado, infectado, que haya sido usado para alguna actividad delictiva o que haya sufrido un ciberataque, debemos seguir ciertas pautas o ser cautelosos en ciertos puntos:

- **Una parte de la memoria de un equipo puede ser volátil**, lo que significa que por ser alterada se pueden llegar a perder archivos importantes o relevantes para la investigación.

- **Debemos evitar alterar el equipo**. Debido a la cadena de custodia, el equipo se convierte en evidencia útil para los jueces o abogados que la requieran como pruebas. El hecho de trabajar con este mismo equipo provoca varias alteraciones en su memoria, como, por ejemplo, la pérdida de evidencia válida. Lo que se debe hacer, es hacer una copia de los archivos afectados y del equipo en su totalidad, o usar algún método de contraescritura. Aunque la del equipo no es del todo necesaria, más bien, los archivos necesarios(Dependiendo siempre del tiempo disponible y de los objetivos que se tengan).

- Respecto al punto anterior, también el hecho de usar el equipo original puede llevar a la **pérdida de credibilidad** del mismo perjudicando juicios o asuntos legales.

- Cabe destacar que a veces, la adquisición de evidencia se debe hacer desde el mismo dispositivo afectado por los archivos volátiles, aunque hayamos copiado la máquina , hay archivos volátiles que están en la máquina original. Pero si lo hacemos, nuestra evidencia se verá afectada y puede llegar a perder utilidad.

- Si no se siguen los **procedimientos**, a la hora de hacer el informe “específico”, los pasos no se podrán seguir correctamente, como por la alteración del dispositivo afectado por la carencia de ciertas partes de las pruebas necesarias por ejemplo.

Al llevar a cabo una investigación forense en un dispositivo electrónico hay ciertos puntos a tener en cuenta que pueden ser beneficiosos o perjudiciales a la hora de llevar a cabo desde un punto ético o legal.

## Análisis Forense Digital {###-análisis-forense-digital}

### Ventajas y desventajas {####-ventajas-y-desventajas}

- Ventajas: Son las características de la investigación que ayudan a la obtención de evidencias, facilitando el proceso. Esto engloba lo útil que es llevar a cabo una investigación forense digital.

  - Es muy útil para llegar a resolver casos largos y difíciles, como crímenes que se han estado llevando a cabo o encontrar pruebas en el juicio.  
  - La recopilación de evidencias digitales es más eficaz gracias al uso de diferentes programas útiles que ayudan a recuperar información eliminada o conseguir nueva información.   
  - La probabilidad de encontrar pruebas útiles aumenta (Login, dirección, etc). Hoy en día , los dispositivos electrónicos almacenan toda clase de información que puede ser útil.  
  - Debido a la complejidad de algunos crímenes, la digitalización general ayuda a facilitar la búsqueda de responsables y culpables, incluso si son crímenes ya cometidos (Un móvil de un delincuente, un ordenador encontrado en una escena, un USB, etc), debido a que una gran mayoría de estos se dejan pruebas y evidencias en los dispositivos.

- Desventajas: Son las limitaciones que ralentiza o perjudica en cierta manera la investigación. Indica los inconvenientes que pueden surgir al llevar a cabo una investigación forense digital.

  - Problemas con la privacidad legales. El hecho de analizar un equipo ajeno, por mucha evidencia que pueda contener, se pueden encontrar archivos personales que no están relacionados con el análisis que se está realizando. Esto aparte de no ser legal, entra en un debate ético por la investigación.  
  - Muchos riesgos al recopilar la evidencia si no se siguen los procedimientos adecuados. Las evidencias obtenidas pueden perder veracidad si se trabaja sobre el mismo equipo, o hasta se pueden perder evidencias si no se tiene presente algún método de contraescritura.  
  - Si se trata de dispositivos anticuados, la obtención de evidencias se puede ver comprometida.  
  - No siempre se puede recuperar toda la evidencia, si, por ejemplo, el hardware está dañado será inútil intentar analizarlo, en la mayoría de casos, ya que si es posible recuperar algo de la información , se puede intentar sacar algo, pero es muy poco probable y no es recomendable hacerlo.

El análisis forense digital es necesario llevarlo a cabo en ciertas situaciones que se pueden considerar graves o cruciales dependiendo del contexto:

- En ciberataques que hayan acabado determinados como graves o que incluyan información confidencial: Esto se debe a que ya que se han catalogado como graves, será debido a que la información afectada es importante o podría estar en juego. Usando las herramientas correctas, se puede sacar información del análisis tras (o durante) un ataque, ya sea, por ejemplo, una dirección, la manera en la que el ataque ha iniciado(que ayuda a futuras defensas), etc. 
- Delitos: Si se diera el caso de que algún dispositivo electrónico este relacionado con un crimen, es conveniente analizarlo siempre que se respeten ciertos derechos de la privacidad si es un dispositivo personal, es decir, se debe hacer siempre que se hayan revisado y obtenido permiso para llevarla a cabo para evitar toda clase de problemas legales. El objetivo será la recuperación de archivos que ayuden en la investigación (que hayan sido eliminados) o en encontrarlos (que no hayan sido eliminados) o puede ayudar a sacar información “oculta” en un primer lugar. Esto puede ayudar en diversas investigaciones de crímenes o incluso en juicios para incriminar al culpable.

El hecho de invertir tiempo en estas investigaciones es bueno, y recomendable en el trabajo, ya que se puede ayudar a recuperar datos o a mejorar la defensa de sistemas informáticas frente a posibles ataques.  
Sin embargo, hay casos en los que no es rentable hacer una investigación completa, ya sea:

- En casos con demasiado poco tiempo no es rentable empezar una investigación principalmente por la falta de tiempo, sin embargo, si se requiere se puede intentar hacer. Ya que , por decirlo de cierta manera, hay mucha oferta (Trabajos relacionados, investigadores, etc) y poca demanda (refiriéndome a los analistas forenses) ya que considero que es un campo muy requerido y que es necesario centrarse en los casos mas graves.

Una aclaración es que los puntos de vista pueden variar debido al tiempo que se le ha dado a un investigador forense digital para analizar, obtener evidencias y realizar informes que ayuden en una investigación.  
Para concluir esta parte, las ventajas son una de las mayores virtudes de este tipo de investigación gracias a la facilidad para recuperar o conseguir información de crímenes o caos juridiciales.

## Directrices de las fuerzas de seguridad  {###-directrices-de-las-fuerzas-de-seguridad}

En las investigaciones/análisis forenses digitales, se suelen aplicar ciertas directrices que vendrían siendo los procedimientos o protocolos que se deben llevar a cabo para garantizar la veracidad de las pruebas en casos judiciales, por ejemplo. Estos procedimientos se llevan a cabo para, aparte de mantener la veracidad de las pruebas, cumplir con los principios éticos y legales. Algunas directrices que se suelen aplicar son:

- Interpol: Establece procedimientos usaos generalmente para la recolección y análisis en casos en los cuales se deba usar un análisis forense digital. Estando diseñadas estas directrices para un contexto global , es decir, todos los países deberían poder usar las directrices que se establecen y en un principio no son obligatorias estas regulaciones. En un principio pudiéndose usar por las fuerzas de seguridad de un país, o por equipos de ciberseguridad a los que se les haya dado un caso específico de análisis forense digital. La organización interpol  muestra:  
  - Procedimientos para dirigir un laboratorio forense digital  
  - Guías que muestran procesos de búsqueda de evidencias y como manejarlas para mantener su integridad

  (Interpol, s.f.)

- RFC 3227: Esta clase de documentos (RFC), son documentos que recogen propuestas de expertos para ayudar a mejorar en ciertos casos ,con una serie de pasos o procedimientos a seguir, los procesos de análisis forenses. Estos procesos son recomendados, no obligatorios, y los puede usar en varios países (EEUU, España, México, etc) como una buena práctica. Este documento establece algunas prácticas como:  
  - Principios durante la recolección de evidencias  
    - Imágenes del sistema precisas  
    - Documentación detallada  
    - No hacer cambios en la información recolectada  
    - Tener en cuenta el orden de volatilidad(Recoger la información volátil primero)  
  - Procedimiento de recolección  
    - Usar métodos de recolección repetibles   
    - Determinar lo relevante, fijar orden de volatilidad, comprobar la sincronización de la hora del sistema  
  - Procedimiento de almacenamiento  
    - Cadena de custodia: Buena documentación de:  
      - Los recolectores de la evidencia, como y cuando la recolectaron  
      - Los que han analizado la evidencia, cuando y como  
      - Quien ha guardado la evidencia original y como   
  - Herramientas necesarias  
    - Usar herramientas ajenas al sistema (Por malware)  
    - Usar herramientas que no alteren la evidencia

(Martínez, 2014)

- ISO 27037: Por decirlo simple, “renueva” el RFC 3227 orientándolo a dispositivos actuales. Esta metodología está orientada a la recolección, identificación y secuestro de la evidencia digital (sin entrar en la fase de análisis forense). También establece que la evidencia que se puede recopilar digitalmente es:  
  - Correos electrónicos  
  - Mensajes  
  - Transacciones  
  - Imágenes  
  - Historiales

Esta metodología establece directrices para la identificación, adquisición y la preservación de la evidencia digital teniendo varios aspectos particulares:

- Evidencia digital  
  - Motivación de una investigación  
  - Evidencia que se puede recopilar digitalmente   
  - Como se desarrolla la adquisición  
  - Como y donde se desarrolla el análisis

  La ISO 27037 establece que la evidencia digital son los datos o la información de valor que se almacena, recibe o transmite por medio de un dispositivo electrónico. Establece que la evidencia digital:

  - Está oculta, como huellas digitales  
  - Cruza fácilmente fronteras jurisdiccionales   
  - Puede ser alterada de diversas maneras  
  - Puede ser sensible al paso del tiempo

  Debido a que la información se almacena en dígitos, los cuales representan diferentes tipos de archivos, hay unos aspectos principales a tener en cuenta en la investigación.

  - Ordenadores: La evidencia digital se suele encontrar en el disco duro, USB, discos duros externos, …  
  - Internet: Los criminales los suelen usar para llevar a cabo actividades delictivas, por ende, los investigadores deben de estar a día de los avances tecnológicos   
  - Dispositivos móviles: Los dispositivos ya que cada día se usan más, pueden llevar un registro de las actividades llevadas a cabo por los criminales

Se establece que la evidencia digital almacenada, recogida y presentada debe ser:

- Importante/Útil  
  - Fiable  
  - Suficiente

La norma también presenta la cadena de custodia, que consiste en establecer los recaudos mínimos a tener en cuenta:

- Un identificador de la evidencia  
  - Quien, cuando y como se accede a la evidencia  
  - Los procesos del paso de la evidencia

Se establecen unas normas en esta norma para la adquisición de evidencias:

- Asegurar la escena  
  - Confirmar las autoridades legales  
  - Recopilar las contraseñas/códigos…  
  - Mantener la cadena de custodia en todo momento  
  - Preservar condiciones físicas optimas de la evidencia original (Para que no se deteriore)

También recoge normas para el posterior análisis de las evidencias:

- Evitar la contaminación de las evidencias originales  
  - Mantener el estado original de la evidencia original  
  - Aislar los dispositivos inalámbricos  
  - Tener y usar un programa de bloqueo de escritura  
  - Las evidencias digitales se deben analizar como evidencias físicas(Huellas, ADN,…)

(Martínez, 2024)  
Esta “metodología” tiene varios principios:

- **Aplicación de métodos:** Dice que la evidencia se debe adquirir de la manera menos intrusiva posible intentando mantener la evidencia original intacta y creando copias de repuesto.  
  - **Proceso auditable**: Los procedimientos deben de ser bien documentados, y dicha documentación debe haber sido validada por las buenas prácticas.  
  - **Proceso reproducible:** Los métodos aplicados deben ser reproducibles, verificables y argumentables con un buen nivel de comprensión del campo.  
  - **Proceso defendible**: Se deben mencionar las herramientas usadas, y deben de haber sido validadas

(Rafael, 2012)

- ISO 27042: Siendo esta una guía para el análisis de evidencias digitales, establece directrices a seguir de cómo abordar el análisis y la interpretación de las evidencias digitales. Esta norma declara indicaciones de que se debe incluir en el informe siempre que no haya problemas o restricciones legales:  
  - **Información inicial de la que se dispone**  
  - **Fecha/Hora/duración del incidente**  
  - **Objetivos de la investigación**  
  - **Miembros del equipo**  
  - **Fecha/Hora/duración de la investigación**  
  - **Hallazgos de la investigación**  
  - **Daños en la evidencia**   
  - **Detalles de los procesos/herramientas**  
  - **Conclusiones**  
  - **Recomendaciones a futuras prácticas**

Esta metodología aporta resultados fiables y solidos a la hora de presentarlos, validando la evidencia presentada en los tribunales. Esta norma se puede decir que es esencial en las investigaciones forenses digitales. También hay casos en los que la preservación de la evidencia original se puede ver afectada, debido a esto, se han ideado regulaciones o métodos para ambos métodos de análisis:

- Análisis estático: Se lleva a cabo una investigación a fondo, dentro del tiempo dado , llevando a cabo una documentación detallada y precisa.  
  - Análisis en vivo: Estos casos suelen ser en casos volátiles, y es útil para obtener una imagen de la situación. Se inspecciona la RAM, los mensajes enviados y se analizan comportamientos sospechosos en tiempo real.

(Gonzalez, 2015)

- OLAF: Define qué es una operación forense , bases digitales en Europa para las investigaciones forenses , sobre los datos personales, procedimientos que se deben seguir,etc. En primer lugar, estas “pautas” establecen que una investigación forense digital es la inspección tecnológica , adquisición y análisis de medios digitales/contenidos , usando equipamiento de análisis forense y herramientas adecuadas con el objetivo de encontrar, identificar, recopilar y obtener datos relevantes para la investigación.  
  - **Investigaciones internas**: OLAF se define, en el artículo 4 de la regulación 883/2013 de la UE, como la organización a cargo de la obtención y desarrollo de investigaciones forenses digitales con soporte a grupos ajenos legales. Dichos grupos tienen la obligación de cooperar con OLAF en el campo del análisis forense digital  
  - **Investigaciones externas**: En el artículo 3 de la regulación 883/2013 de la UE, se define que OLAF debe tener acceso a todos los datos y documentación de una investigación

También , OLAF, establece que si los dispositivos analizados contienen datos personales que no son relevantes para dicha investigación, los analistas e investigadores forenses deben respetar los principios de legitimidad , necesidad y proporcionalidad en el contexto de la investigación  
(Martínez, 2024)

- NIST SP 800-61:Siendo el Instituto nacional de estándares y tecnología(National Institute of Standarts and Technology), establece recomendaciones que se deberían de seguir a la hora de gestionar incidentes. Explica la necesidad de establecer responsabilidades y organización a la hora de responder a incidentes, incluyéndose aquí las investigaciones forenses.  
  (Martínez, 2024)  
- CCN-STIC 817**:** Siendo este el centro criptológico nacional, es un organismo conjunto al centro nacional de inteligencia, el cual es el encargado de informar de las directrices y asegurar el cumplimiento del esquema nacional de seguridad en la administración pública. La guía 817 define las prácticas, procedimientos y RRHH de los que se debe contar a la hora de llevar a cabo un análisis forense.

(Martínez, 2024)  
Por lo general, los centros de seguridad de varios países, a la hora de llevar a cabo análisis o investigaciones forenses digitales, deben de seguir ciertos principios, algunos mencionados anteriormente, para reafirmar la calidad y veracidad de la investigación llevada a cabo.

- Cadena de custodia: La evidencia se debe documentar de manera adecuada, atribuyendo las respectivas responsabilidades a las diferentes personas que lo llevaron a cabo  
- Integridad de la evidencia: Usar un hash para el volcado de memoria es una buena práctica a la hora de llevar a cabo una investigación , al principio y al final, para así poder saber si el volcado de memoria es diferente respecto al principio, y por ende, que haya sido alterada.  
- Usar herramientas correctas y legales: Uso de FTK Imager  ,Autopsy, o volatility para llevar a cabo los análisis

### Ético {####-ético}

También, antes de llevar a cabo una investigación, se deben tener en cuenta algunos posibles problemas legales o éticos que se pueden llegar a producir si no se tienen en cuenta antes de llevar a cabo una investigación. Al mismo tiempo, estas verificaciones previas de los requisitos legales y éticos ayudan a la veracidad de las evidencias o al caso en general.

- Dependiendo del país del que venga el acusado o donde se haga la investigación, se deben respetar las regulaciones legales que haya en dicho país, ya que en diferentes países puede haber diferentes regulaciones legales respecto a la privacidad de las personas. En estos casos, lo mejor sería asegurarnos y establecer límites para evitar incumplir las leyes de otros países de la privacidad, u obteniendo permisos legales necesarios para llevar a cabo la investigación si se puede.  
  Como en España , por ejemplo, el reglamento general de la protección de datos(Dependiendo del caso si es individual o de una empresa), el cual define qué es un dato personal, también habla sobre los derechos de los individuos(derecho al acceso, oposición[Si se niegan a dar los datos],corrección,…), y también habla del tratamiento de los datos en si(Usar los datos de manera justa, se deben recoger solo los datos necesarios para el tratamiento, confidencialidad,…)  
  (europea, 2016)

- Aun así, también, respecto a los puntos éticos de la investigación, lo suyo sería:  
  - Evitar incluir información que no tenga que ver con el caso en el informe, ya que , puede no ser relevante para la investigación, o abarcar puntos personales del investigado que le podrían afectar negativamente en otros aspectos ajenos a la investigación  
  - No revelar información personal/privada no relevante para el caso, siguiendo con el anterior punto, tampoco se pueden mencionar en una conversación ya que se violarían varios valores de privacidad  
  - Se debe obtener consentimiento, al menos legal, para poder acceder a las evidencias  
  - La información obtenida no se debe usar para empeorar la reputación de la persona analizada ya sea social o judicialmente si no se requiere

(Duriva, 2023)   

[GitHub: Ch4mbi](https://github.com/Ch4mbi)

# Investigación Forense Digital {##-investigación-forense-digital}

En el escenario que nos ha dado, los policías han arrestado en el aeropuerto de Wellington del vuelo entre Nueva Zelanda y Brisbane a dos personas. Los arrestados eran John (Narcos-2) y Jane (Narcos-3) ya que se sospecha de que han llevado a cabo algún tipo de actividad ilegal, como narcotráfico. En ambas maletas se ha encontrado un ordenador portátil y en la de John se ha encontrado droga. Jane confesó que debían dejar la maleta en la biblioteca de Eastbourne(Wellington), y John lo corroboró.Una vez ahí, solo encontraron armas, drogas y un portátil. El informe consiste en relacionar a los detenidos con el sospechoso Steve y las actividades que se han intentado llevar a cabo o que se harán, al menos establecer una relación entre Steve y John.   
Yo debo entender y hacer una conclusión de:

- Qué ha pasado   
- Cuales han sido los efectos  
- Como se ha producido  
- Sobre qué dispositivos ,redes, o sistemas ha tenido lugar la acción o el ataque  
- Autoría(Quienes son los responsables)

Una investigación forense tiene un proceso que se suele repetir en todas:

1. Recopilación de evidencias  
2. Adquisición   
3. Análisis  
4. Reporte

Al mismo tiempo, un proceso de análisis forense lleva una serie de pasos a seguir:

1. Desarrollo e políticas  
2. Evaluación e identificación de evidencias  
3. Adquisición de evidencias(Redactando lo que se hace paso por paso y usando métodos de contraescritura para asegurarnos de que no han sido alterados los archivos)  
4. Análisis  
5. Documentación

## Planificación {###-planificación}

Para esta investigación de Narcos , se van a usar diferentes herramientas como:

- Autopsy: Aplicación que sirve para el análisis de un disco, ya sea , imágenes, historial, descargas,…  
- FTK imager: Aplicación  usada para analizar el contenido de un dispositivo de manera organizada y por carpetas de manera más interna  
- Volatility: Aplicación que sirve para hacer un análisis de la memoria volátil de un dispositivo  
- HashMyFiles: Aplicación que genera uncódigo único en textos o archivos  
- OpenStego: Herramienta usada para esconder o desentrañar secretos en archivos como imágenes o documentos

En la investigación se van a usar imágenes de las aplicaciones usadas, pero no cuentan como evidencia, solo como referencia y guía para que otros puedan llegar a las mismas conclusiones.  
Cada aplicación puede servir para cada una de las fases de un análisis forense.

- Fase de recolección:   
  - FTK Imager  
  - HashMyFiles  
- Análisis:  
  - Autopsy  
  - FTK Imager (En situaciones especificas, normalmente no se usa en la fase de analisis)  
  - Volatility  
  - [OpenStego](https://www.openstego.com/)(Para un intento de análisis puntual)  
- Adquisición de evidencias  
  - FTK Imager  
  - HashMyFiles(El hash será igual siempre y cuando no se haya alterado el archivo del que se ha hecho el hash. Sirve para comprobar la integridad de los documentos y que no hayan sido alterados)

Hay que tener en cuenta los dispositivos con los que se va a trabajar en la investigación:

- Los ordenadores, no se va a trabajar directamente con ellos(hardware) debido a los riesgos que supone de alterar la evidencia original , por lo que se va a trabajar con un volcado de memoria de cada uno:  
  - Ordenador de Steve(Narcos-1)  
  - Ordenador de John(Narcos-2)  
  - Ordenador de Jane(Narcos-3)  
- Los 3 ordenadores se van a analizar en mi ordenador personal, usando las aplicaciones debidas para su análisis o recolección de evidencias:  
  - FTK Imager(Recolección)  
  - Autopsy(Análisis)  
  - HashMyFiles(Recolección)  
  - OpenStego  
  - Otras herramientas si se requieren a la hora de investigar si es necesario  
  - Para el reporte del caso,  se llevará a cabo un word en el que contenga los pasos a seguir para replicar la investigación correctamente

Tras haber analizado con FTK Imager los 3 dispositivos, se ha llegado a una conclusión respecto a cómo se organizan internamente, esto parece ser un sistema de carpetas dentro de otras para llegar a archivos importantes. Y según las rutas usadas para navegar entre carpetas entre los 3 dispositivos individualmente, se puede intuir que los 3 son sistemas Windows.

## Comparación de herramientas  {###-comparación-de-herramientas}

Comparación de herramientas de análisis forense(Fase de análisis):

| Autopsy | FTK Imager |
| :---- | :---- |
| 
- Interfaz fácil de usar e intuitiva(desde la experiencia y desde mi punto de vista), ya que tiene diversas opciones para organizar las búsquedas, como una sección para buscar archivos por su nombre<br><br>
- Es lento, por decirlo de una manera, tarda en analizar todo la memoria analizada un rato ya que es una herramienta que se especializa en los analisis detallados por lo que tarda más en analizar toda la información<br><br>
- Muestra toda la información de los volcados de memoria<br><br>
- No solo permite ver imágenes en “secciones” según la clase de imagen que sea, sino que también se pueden ver descargas de internet, cookies, sitios web visitados, etc. | 
- Interfaz más extensa y compleja, dividiendo los archivos en más secciones separadas, y , por ende, se necesita saber dónde mirar en un primer lugar<br><br>
- Es inmediato, una vez que se cargan las evidencias , ya se puede empezar a interactuar con ellas<br><br>
- Las secciones de archivos ayudan a entender con qué clase de sistema operativo se está trabajando<br><br>
- Su función principal es la adquisición de evidencias,ya que no muestra todas las imagen(por ejemplo) del disco, pero se puede usar para un análisis inicial y contrastar información |


## Funcionamiento del sistema operativo  {###-funcionamiento-del-sistema-operativo}

Todos los sistemas operativos tienen una lista limitada de sistemas de archivos compatibles. En este primer caso, va a analizar este tipo de estructura de Windows ya que este análisis forense se  enfoca en dispositivos lo que parece ser dispositivos windows:

- NTFS(New Technology File System ): Introducido en Windows NT, hoy en día es el sistema de archivos más común. NFTS es en varios puntos mejor que FAT, dando diferentes funciones como: control de acceso, compresión de archivos,…También usa estructuras de datos específicas para aprovechar el almacenamiento:  
  - *$Boot*: Está presente en el proceso de arranque  
  - *$MFT*: Tiene una entrada para todos los ficheros, los cuales pueden tener cualquier tipo de información, del sistema. Si el archivo es demasiado grande, NTFS crea clústeres fuera de la MFT, y punteros a las ubicaciones de dichos clústeres.

  - *$Bitmap*: En este archivo se registran los estados de los clústeres , cada bit dentro representando un clúster(1 Cuando está ocupado y 0 cuando está vacío/libre/no ocupado).  
  - *$Logfile*: Este archivo sirve a modo de registro. Al alterar la estructura del sistema, este archivo registra los cambios en los clústeres. De esta manera, si sucede algún tipo de error, se pueden recuperar antes del error.  
  - *$BadClus*: Siguiendo con el punto anterior ($Logfile), en caso de error, el NTFS registra el clúster errático y copia los datos en otra ubicación.  
  - *$Recycle.Bin*: Esta carpeta almacena los archivos eliminados de manera temporal antes de su eliminación final.  
- FAT/FAT32/exFAT(File Allocation Table):Almacenamiento de baja capacidad de mente. Su sistema de archivos se basa en una tabla , mostrando su contenido.  
  - **Sector de arranque**: Primer sector en cualquier partición formateada con FAT, conteniendo información importante sobre su organización.  
  - **Tabla de asignación de archivos**: Asignación de archivos FAT principal, así como su “copia de seguridad” a la cual se pueden acceder en caso de un problema con la lectura del original.  
  - **Área de almacenamiento de datos**: La mayor parte se divide en clústeres (usado como una unidad mínima para la asignación de archivos).Un archivo ocupa todo el clúster, desperdiciando el espacio sobrante. Cuando se necesitan varios clústeres ,puede asignarse una cadena consecutiva provocando la fragmentación del archivo.

  El número del FAT, representa el número de bits para cada clúster. Hoy en día se usa FAT32(32 bits) por su amplia compatibilidad. También se creó exFAT(extended File Allocation Table), debido a que FAT32 no cuenta con la capacidad mayor a 32 GB, por lo que el exFAT no tiene limitaciones respecto a su tamaño y normalmente usa los discos duros externos.

- ReFS (Resilient File System): Se creó para abordar problemas del NTFS, principalmente respecta a la corrupción de la información almacenada. Este sistema , a diferencia del NTFS, este sistema , al editar los datos de la información, guarda la copia en otra zona del almacenamiento, y en lugar de sobrescribirla la información en ese mismo sitio, la actualiza y la vincula a la copia en el otro sitio del almacenamiento. De esta manera, muchas copias se almacenan en diferentes sitios de la memoria facilitando su restauración en caso de eliminación o corrupción. ReFS está diseñado para sistemas de almacenamiento grandes, pero no se considera tan estable como el NTFS.  
- *HPFS*(High Performance File System):Busca , con los clústeres ,crear bloques unidos , o al menos que los archivos estén mas cercanos entre sí. Al comienzo, hay 3 bloques que ocupan 18 sectores:  
  - **Bloque de arranque**  
  - **“Super bloque”**  
  - **Bloque de repuesto**

El espacio sobrante se divide en sectores contiguos de 8MB cada uno. Cada directorio tiene su propio F-nodo, ubicado cerca en el mismo disco, conteniendo información de la localización del archivo y sus atributos. Aun así, debido a que tenia limitaciones, hoy en día está obsoleto.  
(Explorer, s.f.)  
A la hora de llevar a cabo un análisis forense, hay que usar herramientas adecuadas para poder hacer un análisis efectivo del dispositivo. Al usar algunas de estas herramientas hay que tener en cuenta los artefactos del sistema de ficheros, como cuando usamos, por ejemplo, FTK Imager. Normalmente, algunos ficheros de interés son:

- $MFT: Ya mencionada antes, es una base de datos en la cual se guarda la ubicación del sistema de ficheros, metadatos y permisos. Debido a que todo lo que se graba en un disco se considera un fichero, cualquier tipo de modificación quedará registrada en el MTF   
- $I30: Es un índice que relaciona cada archivo con la posición en el disco  
- $Logfile:Es un registro sobre las últimas acciones llevadas a cabo sobre el sistema de ficheros  
- $MFTMirr: Copia los 4 primeros registros de la MFT  
- $UsnJrnl: Es un registro de los cambios de la MFT

El registro de Windows se divide en 4 hives de sistema y 2 de usuario.

- Hives de sistema:  
  - SYSTEM: Son los datos generales del sistema operativo  
  - SAM:Son los datos de los usuarios  
  - SECURITY: Contiene los datos de seguridad del sistema  
  - SOFTWARE  
- Hives de usuario  
  - NTUSER.DAT: Contiene las configuraciones del usuario  
  - USRCLASSDAT:Su importancia está en las shellbags(Almacenan información sobre las carpetas que un usuario ha abierto en el explorador de archivos)

Los eventos de Windows suelen incluir mensajes de errores, de aplicaciones, del sistema, …Siendo útil para solucionar problemas o al menos para tener constancia de ellos. En sistemas posteriores a Windows Vista/7/2008 , los eventos quedan almacenados en ficheros EVT.  
(Martínez, 2024)

## HashMyFiles {###-hashmyfiles}

Narcos-1  
Usando HashMyFiles, se pueden sacar los Hashes MD5 de los archivos de Narco_1:  
En las carpetas inicialmente hay 2 carpetas:  
![img1](img/img1.png)

- En un primer lugar, se hace un hash de las imágenes que venían en la carpeta:

![img2](img/img2.png)
- Después , se hace del Memory Dump

![img3](img/img3.png)
Narcos-2

- Images

![img4](img/img4.png)

- Memory Dump

![img5](img/img5.png) 
Narcos-3

- Image

![img6](img/img6.png)
- Memory Dump

![img7](img/img7.png)

Pasos para abrirlos en autopsy  
A la hora de analizar el equipo, se debe abrir en Autopsy, creando un nuevo “proyecto”, poniendo el nombre deseado, en este caso de estudio, sen han elegido las siguientes opciones de analisis:  
![img8](img/img8.png) 
![img9](img/img9.png) 
Después se selecciona la carpeta de Narcos_1  
![img10](img/img10.png)
![img11](img/img11.png)

# Escenario

"Due to intelligence provided by the Australian government, two passengers were intercepted by
Customs upon arriving in Wellington, New Zealand from Brisbane. The Intel stated that Jane
Esteban and John Fredricksen may be involved in illegal activity.
The suspects were each searched by a customs officer. John Fredricksen’s baggage consisted
of clothing, toiletries and a Windows laptop. Jane Estebans baggage also consisted of clothing,
toiletries and a small windows laptop.
Upon further search of the lining of the suitcase, one kilogram of Methamphetamine was
located. Both suspects were taken into separate interview rooms where they were interrogated.
John Fredricksen refused to answer any questions.
Jane Esteban stated all she knew was that she had to deliver the suitcase to the “Eastbourne
library” but if all else failed then they were to deliver it to 666 Rewera Avenue, Petone as told by
John.
Customs and police subsequently raided that address. There was nobody present at the
address. Customs did, however, find drugs, guns and a desktop computer in the living room of
the suspects house.
You are a Customs forensics investigator. Customs officers have delivered images and memory
dumps of the 2 laptops and 1 desktop computer to you. Your task is to carry out a forensic
examination of John Fredricksen, Jane Esteban and the unknown suspect’s laptops and
desktop computers to further understand their motives, goals and objectives. It should be noted
that all three devices contain different Windows 10 builds and resulting artefacts may not be
located in the same location or even be present."

https://digitalcorpora.s3.amazonaws.com/s3_browser.html#corpora/scenarios/2019-narcos/


# Narcos 1 {##-narcos-1}

Primero se va a analizar la carpeta de Narcos-1, la que contiene información de Steve.Se sabe el nombre por las rutas de acceso a los diferentes archivos que aparecen en autopsy. El dispositivo parece ser un sistema windows.  
Usando FTK Imager, e investigando la carpeta de Narcos-1.001, en la sección de Basic Data Partition,en la sección de Noname, en la carpeta root, en la carpeta $Recycle.Bin , en la subcarpeta S-1-5-21, se han encontrado una serie de imágenes jpg con contenido de drogas.

## Primeras Imágenes de drogas {###-primeras-imágenes-de-drogas}

Analizando la organización de las carpetas, por medio de FTK Imager, se puede deducir que se trata de un sistema windows, aparte de las carpetas del sistema operativo de windows, se ven carpetas relevantes como $Recycle.Bin.  
![img12](img/img12.png)
![img13](img/img13.png)
![img14](img/img14.png) 
Esta imagen está junto con la otra imagen de drogas de Steve. En ella se pueden ver chaquetas de una pandilla callejera criminal de Nueva Zelanda.  
Estas imágenes se han encontrado en la carpeta $Recycle.Bin del ordenador de Steve, siendo esta carpeta usadas para , en este caso, encontrar archivos que el dueño del ordenador ha intentado eliminar, ayudando en la investigación debido a que nos indica que ha intentado deshacerse de algo que lo podría incriminar.Esto , y el análisis por medio de FTK Imager, de la visualización de todas las carpetas, se puede lograr ver que muchas carpetas se encuentran dentro de otras carpetas,, por lo que se puede deducir que esa es la forma en la que se organiza este dispositivo(Al igual que los otros 3)

## Mapas {###-mapas}

Usando autopsy y analizando Narcos -1.001, en la sección de imágenes se pueden ver imágenes de google maps de la zona de wellington:  
![img15](img/img15.png) 
En autopsy se puede ver como ha llamado al archivo : Airport Crystals  
![img16](img/img16.png) 
También se ha encontrado una imagen del google maps en la que Jane decía que había droga, en la biblioteca. Habiendose encontrado en la carpeta de documentos del ordenador de Steve, usado FTK Imager.Esta carpeta normalmente se usa para almacenar documentos personales, ya pueden ser archivos de texto, imágenes, por lo que no es raro encontrar imágenes relevantes en esta carpeta o que puedan dar apoyo en la investigación. Y el contraste, aunque no se usan para la misma fase de análisis forense,entre Autopsy y FTK Imager, nos permite entender en mayor medida qué documentos ha intentado ocultar o donde están guardados.  
![img17](img/img17.png)

![img18](img/img18.png)  
Y es posible que el usuario haya tomado una captura de pantalla a una ubicación importante, una calle que posiblemente se encuentre en algún lugar de wellington.  
![img19](img/img19.png) 
Pero es difícil saber donde es esa imagen ya que no parece haber ningún punto de referencia más que las calles, que están demasiado borrosas. Se ha conseguido ver el nombre de una de las calles ,Wakefield Street, que es la más próxima al marcador de la imagen. Según Google maps, parece ser una plaza o una galería, no se sabe más información sobre este punto más que parece estar cerca del ayuntamiento.  
Y hay un lugar en el cual la imagen pone casa, pudiendo ser la casa de Steve o un punto de recogida(La biblioteca)  
![img20](img/img20.png)
En la imagen también se ven rutas a diferentes ciudades: Stokes Valley, Naenae y Wainuiomata. A lo mejor son rutas de venta de drogas, de ahí que se llame method.  
Este se ve en Ftk imager como methodpoff , indicando una posible ruta de escape o el método que debe seguir:  
![img21](img/img21.png)  
El hecho de que ambas imágenes se puedan encontrar en ambas herramientas ayuda al contraste de imágenes ,ya que con Autopsy, solo se pueden ver, y es más difícil saber con exactitud dónde está cada imagen. Por ejemplo, también, en cierta manera, el hecho de que no esté en la carpeta de descargas nos puede dar a entender que el documento fue creado y guardado por Steve.

## Billete {###-billete}

También se pueden encontrar imágenes de un vuelo del 16 de febrero habiendo sido creadas el día 2. Esto da a entender que ha habido un tiempo de preparación y que el lapso de sucesos ha ocurrido entre finales de enero y principios de febrero de 2019.  
![img22](img/img22.png) 
El billete no tiene porqué haber sido de Steve necesariamente, los que han cogido un avión eran John F y Jane E

## Búsqueda de drogas {###-búsqueda-de-drogas}

También en la sección de webp, se pueden encontrar numerosas imágenes de compra de drogas en tiendas digitales con fecha el 2 de febrero  
![img23](img/img23.png)  
![img24](img/img24.png)

## Historial {###-historial}

Usando también autopsy, se ha encontrado también un historial de búsqueda que son sospechosas, como: Crystal meth, best places to trade drugs  
![img25](img/img25.png)

![img26](img/img26.png) 
Al mismo tiempo, parece que buscaba un lugar para vender las drogas:  
![img26](img/img27.png) 
Esto podría coincidir con que Steve vaya a vender las drogas en los lugares marcados en el mapa en el que pone home:

![img27](img/img28.png) 
Y es posible que hayan usado discord como medio de comunicación aparte de gmail u otros más comunes  
![img28](img/img29.png) 
Como discord, como se puede ver en la búsqueda.  
Entre otras búsquedas como sobre cómo lavar dinero, taxis por la zona de Wellington, y rutas de drogas por la zona.

![img29](img/img30.png) 
Discord se usó el mismo dia que se instaló , coincidiendo con el lapso de tiempo entre enero y febrero

Sin embargo, usando FTK Imager, y autposy para contrastar información, se ha encontrado algo que podría ser importante. Primero en autopsy, se ha encontrado en Data artifacts- Web Downloads, abajo, se ha encontrado una descarga de una serie de imágenes, las cuales, usando FTK Imager,se pueden visualizar por la carpeta donde están ubicadas.  
Autopsy:  
![img30](img/img31.png) 
Como se ve, en la imagen , el archivo seleccionado y los que están arriba, tienen una ruta similar. En autopsy no se puede ver, pero si seguimos la ruta en FTK Imager,se pueden ver las imágenes que mostraban drogas anteriormente creando la posibilidad de que no hayan sido tomadas por el usuario del ordenador, sino que hayan sido descargadas de páginas web o que sean una descarga desde una aplicación de mensajería ya que es necesario, aunque sea desde una pagina web de internet como gmail, whatsapp, etc., se deben descargar.  
![img32](img/img32.png) 
Como se ve , estas carpetas que contienen estas imágenes, están en la $Recycle.Bin, por lo que podrían haber sido puestas ahí para distraer o para incriminar a otra persona, o que hayan intentado eliminarlas.Se puede suponer que son falsas por el link del que se descargaron, ya que los 3 son diferentes. Aun así, es posible que se haya usado algún método especial.Se sospecharía más si se hubieran descargado de la misma página. Es posible que no sean imágenes de John , sino de la propia banda de Steve todas.

# Narcos 2 {##-narcos-2}

Ahora se va a analizar la carpeta de Narcos-2, que corresponde a John F.

Aprender encriptación  
Se encuentra una búsqueda para aprender a encriptar por medio de youtube. Por lo que lo podría haber usado para aprender a encriptar archivos o documentos.  
![img33](img/img33.png)

## Billete {###-billete-1}

También se encuentra el billete de vuelo que previamente poseía Steve.  
![img34](img/img34.png) 
El hecho de que la imagen del billete se llame Steve K, da lugar a 2 opciones, o es la confirmación de vuelo de Steve, o es el billete de vuelo de John F y de Jane para llegar a Steve.  
También hay una confirmación de envío de paquete de 20 kg, a la dirección de 5/34 Hapua Street Remuera Auckland 1050 New Zealand para Jake Heke, un desconocido.  
![img35](img/img35.png) 
En este equipo de John, se han encontrado archivos que llevan el nombre de: Jane´s Kids, siendo esta una imagen. Esto puede dar a entender que John y Jane tienen una relación más cercana, aparte de suponerse por haber sido interceptados los 2 en el aeropuerto.  
![img36](img/img36.png)

## Excel de clientes {###-excel-de-clientes}

Se encuentra también un excel.  
![img37](img/img37.png) 
Por lo que se puede confirmar que Steve era el comprador, y que hacen el envío mensualmente en su caso , o al menos lo pretendían.  
Se confirma que el destino del envío de paquete de 15 kg(de drogas) es a Jake. También se puede ver el nombre de Jane Esteban, el otro sujeto que arrestaron. Se ve como es un envío en proceso de un gramo de “Uppers”. Por lo que Jane podría ser otra consumidora, pero recurrente de John. O que Jane también quiere y está metida con él pero que sea consumidora.Lo que respaldararía la presencia de la imágenes de los niños.  
Todo esto se puede encontrar siguiendo esta ruta en FTK:  Basic data partition → Users → JohnF → Documents →Business  
Cabe destacar que estos archivos no se han podido ver directamente en FTK, por lo que se han exportado 

## Programa de ocultación de secretos {###-programa-de-ocultación-de-secretos}

Se confirma el uso de un programa por parte de alguien para ocultar archivos dentro de archivos “inocentes”.La fecha sigue coincidiendo con el lapso de tiempo entre finales de enero y principios de febrero de 2019.  
![img38](img/img38.png)  
![img39](img/img39.png) 
![img40](img/img40.png) 
Hay imágenes de muchos programas que podrían haber sido usados para la ocultación de textos en imágenes  
Con métodos usados y ejemplos y búsquedas de tutoriales:  
![img41](img/img41.png)

![img42](img/img42.png)  
Y se encuentra un supuesto secreto que ha sido posiblemente encriptado según autopsy  
![img43](img/img43.png)

Se pueden encontrar imágenes creadas en el año 2018, pero que se ha accedido a ellas y modificado de alguna manera.  
![img44](img/img44.png)

## Imagen de localización de drogas {###-imagen-de-localización-de-drogas}

Y una imagen de donde poner las drogas, pero podría ser falsa porque el sitio habitual es alrededor de la biblioteca de Wellington  
![img45](img/img45.png)

## Posibles métodos de ocultación de drogas {###-posibles-métodos-de-ocultación-de-drogas}

Se han visto también diversos alimentos y objetos cortados a la mitad con hueco para esconder cosas.  
![img46](img/img46.png)  
O directamente la posible mercancía en sí  
![img47](img/img47.png)  
Y también imágenes de una maleta abierta, posiblemente la que usa John para transportar la metanfetamina.

## Imágenes de calle {###-imágenes-de-calle}

Se han visto diversas imágenes de una misma calle, y esta apunta a un grupo de casas específico o al vehículo blanco, los cubos de basura, o incluso unas plantas o la carretera de la zona:  
![img48](img/img48.png) 
![img49](img/img49.png) 
![img50](img/img50.png)
![img51](img/img51.png) 
Se han tomado en un corto periodo por las horas a las que se crearon, apenas hay 10 segundos de diferencia entre unas y otras y es curioso las imágenes al suelo que hay, por lo que puede indicar que se han tomado con prisa.

Se vuelve a encontrar en Web Downloads, la presencia de discord y de una aplicación de ocultación/encriptación. El punto es que no es la aplicación como si. Si no que son las imágenes que provienen de un link de donde pone encrypted. Los únicos sitios donde se ve esta alusión a “encrypted” son en 2 imágenes , Drug Memes 5 y 6. Aunque al poner encrypted en lugar de algo relacionado con la esteganografía, que son 2 métodos diferentes, es difícil intuir.  
![img52](img/img52.png)
Y usando FTK Imager y siguiendo la ruta de las imágenes, Basic Data Partition(4) → root → Users→ JohnF → Documents → Memes. Los Drug Memes 5 y 6 están ahí por lo que podrían haber sido usados para la ocultación de información.

## Contact Card {###-contact-card}

Se ha encontrado también un zip llamado Contact card, que parece ser un ejecutable, y otro que se llama Attachments-Important,crucial to our method.zip.Y al ser zip, podrian requerir de una contraseña para descifrarlos.  
![img53](img/img53.png)  
Los zip de Contact card y de Attachments mencionados anteriormente se han descargado desde discord:  
![img54](img/img54.png)

# Narcos 3 {##-narcos-3}

Este ordenador pertenecía a Jane. Parece ser también un dispositivo windows.  
Advertencias de drogas en colegios  
Lo primero que se ha encontrado, es la presencia de imágenes que advierten sobre drogas en colegios.
![img55](img/img55.png)

Se encuentran también numerosas fotos de cristal y de polvos y de metanfetamina, pero que algunas de estas parecen ser de internet por los ángulos y la alta calidad de las imágenes.

## Imagen de grabación {###-imagen-de-grabación}

Una imagen que me parece importante, es esta:  
![img56](img/img56.png) 
Que parecen ser imágenes de una videollamada , o de un hackeo de un teléfono a la cámara del mismo.

## Búsquedas de internet sospechosas {###-búsquedas-de-internet-sospechosas}

Una búsqueda de internet que ha hecho, parece bastante sospechosa:  
![img57](img/img57.png) 
Como aparentar ser y cómo ser físicamente para parecerse a un adicto a la metanfetamina. A lo mejor lo buscó para que no los identificaran como vendedores, sino como consumidores y se sospechara menos de ellos. O que jane tuviera otras intenciones con john , ya que es sospechoso que solo haya comprado un solo gramo.Se les ve una preocupación por la sentencia en prisión que les puede caer por vender o tener alguna relación con los productos.  
![img58](img/img58.png)  
El hecho de que se preocupe de las sentencia en 2 lugares diferentes puede dar a entender de dónde vienen:  
![img59](img/img59.png)  
En este caso hay 2, New Zealand (nz) y Australia(au)  
Se encuentra también una placa de policía en una imagen:  
![img60](img/img60.png) 
Y se encuentra esa foto, pero con extras , con nombre de background  
![img61](img/img61.png) 
Se puede llegar aquí por medio de la siguiente ruta:Basic Data Partition → Root → Users → JaneE → Pictures. Esto nos puede cambiar el punto de vista de las motivaciones de Jane, quitando como compradora, y el hecho de que no conocía a Jhon en un primer lugar, puede ser que Jane sea una policía encubierta en busca de un narcotraficante , Jhon.

## Herramienta sospechosa en descargas {###-herramienta-sospechosa-en-descargas}

Se ha encontrado una herramienta para controlar de manera remota algún dispositivo:  
![img62](img/img62.png)   
![img63](img/img63.png)  
Y aquí se puede ver como lo ha ejecutado  
![img64](img/img64.png) 

## Quasar.v.1.3.0.0 {###-quasar.v.1.3.0.0}

En FTK Imager, se puede ver , junto con el ejecutable en el zip de Contact Card, el programa Quasar v.1.3.0.0. Y parece ser que Jane lo ha usado.  
![img65](img/img65.png)   
En ftk, se puede llegar aquí siguiendo la siguiente ruta:Basic Data Partition → Root → Users → JaneE → Downloads. Se ve como lo ha usado para acceder al ordenador de John.Por lo que a partir de aquí, es más difícil determinar si ha sido John quien ha escrito los mensajes o ha sido Jane por medio de la conexión con el ordenador de John.   
Con el Quasar, se ha establecido comunicación , posiblemente con Steve, por medio de discord:  
![img66](img/img66.png)  
Y a lo mejor , se ha filtrado la contraseña para los archivos de Attachments que se encuentran en el ordenador de John.Este en su ordenador era un .zip, por lo que a lo mejor requería una contraseña , siendo esta: ilovediving.  
![img67](img/img67.png)  
Se confirma el uso de alguna app para la ocultación de secretos en imágenes, y su uso:  
![img68](img/img68.png) 

Se nos da a conocer el nombre de la aplicación que se ha usado para esconder secretos en una o varias imágenes, dice que ha usado una aplicación llamada image steganography.  
![img69](img/img69.png)   
Y parece ser que el archivo lo ha llamado BNE, imagen que se encuentra en el ordenador de Steve. Por lo que se deberá buscar de nuevo en el ordenador de John ya que parece ser él quien lo ha descargado y puesto nombre, y es importante , por el lapso de tiempo que pasa entre la búsqueda de image steganography, y la descarga de la imagen.  
Parece que cambiaron el medio de comunicación, pero se ve igual, la contraseña parece ser Elchapo2.  
Y parece ser que fue John el que compró los billetes de vuelo a Steve.  
![img70](img/img70.png)   
Se confirma que eran los billetes de Steve K, y que han sido comprados desde el ordenador de John F, también se ve como da indicaciones de recogida en: Woolworths (133 Oxlety Station Rd, Oxley QLD 4075)  
![img71](img/img71.png)  
Y se ve como se despide como John, pero podría no ser él y ser Jane.

Cabe la posibilidad de que el archivo Contact card.exe fuera el disfraz que Jane puso al programa para que John lo descargase y tuviera acceso a sus pulsaciones o cámara. Esto se puede suponer debido al ejecutable visto cómo Contact Card.exe en ambos ordenadores.

![img72](img/img72.png)  
Se ve como john parece decirle a Jane que viajarán como una pareja de viaje a nueva zelanda.

## BNE {###-bne}

No se consigue encontrar en el ordenador de John algún archivo con nombre BNE, aun así, en el ordenador de Steve,se encuentra la imagen que John descargó, por lo que John parece haberla enviado y haberla borrado de su ordenador.

![img73](img/img73.png)   
Se puede llegar a ella siguiendo esta ruta: Basic Data Partition → Root → Users → Steve → Downloads → Misc → BNE.

## Intento de descifrar secreto {###-intento-de-descifrar-secreto}

El secreto de la imagen se puede descifrar usando una aplicación de esteganografía, puede ser de elección propia, en este caso se ha usado una llamada [OpenStego](https://www.openstego.com/). La contraseña para la imagen BNE es: Elchapo2. De hecho, OpenStego es una de las imágenes de aplicaciones usadas por John en su ordenador.Siendo la interfaz prácticamente la misma.  
![img74](img/img74.png) 
Comparando la imagen de John, el número de caracteres de contraseña que puso es el mismo que la contraseña Elchapo2, por lo que se refuerza la veracidad de la contraseña.  
Sin embargo, parece que está corrupto el mensaje:  
![img75](img/img75.png) 

## Método de comunicación alternativo {###-método-de-comunicación-alternativo}

Se ha encontrado un sobre con lo que parece cristal dentro, que contiene información de contacto, un gmail, y usan una app llamada Wickr me, que es una app de mensaje directo  privado que “destruye” los mensajes enviados previamente.  
![img76](img/img76.png) 
Por lo que Discord puede haber sido el medio de comunicación casual mientras que Wickr me con el que pasan la mayoría de imágenes o mensajes incriminatorios.

Se puede ver un archivo de Jane que se llama Contact_card.  
![img77](img/img77.png)  
Aunque en este caso es solo un icono, lo que más importa es el ejecutable.  
![img78](img/img78.png) 

# Conclusión {##-conclusión}

En un principio, se pedía que se encontrara una relación entre John y Steve. Pero se analizó también el dispositivo de Jane por si era cómplice, y , de hecho, ha ayudado a la investigación en gran medida.

John Fredricksen y Jane Esteban fueron arrestados en el aeropuerto de Wellington de el vuelo entre Nueva Zelanda y Brisbane.Tras examinarlos, se obtuvo de ellos: 2 ordenadores, drogas en la maleta de John, y una dirección de recogida, una librería de Wellington. Al llegar ahí, se encontraron: armas, droga, y un ordenador. Tras explotarle la memoria, se me dieron a analizar. En primer lugar se examinó el ordenador del desconocido, llamado Steve K. En este ordenador, también se encontraron fotos de drogas, que podrían ser verdaderas debido al uso de discord, por lo que las imágenes se podrían haber pasado por ahí.También se encontraron imágenes de **mapas de la zona de Wellington**, con **rutas** establecidas, la ubicación de la ubicación de la librería,una imagen que parece duplicada de no ser porque en una pone home en la zona de abajo de la ruta que está **marcada con la palabra home**. También se encontró un **billete** de vuelo para el 16-2-2019 de ida a Wellington(Nueva Zelanda) y vuelta el 23-2-2019 de vuelta a Brisbane(Australia).Y también se encontraron en el ordenador de Steve varias imágenes de tiendas online de venta de drogas.Y un historial que muestra preocupación por el tema narcotráfico. También con FTK se encontró una imagen llamada BNE.  
Luego se examinó el ordenador de John Fredricksen. Hay que tener en cuenta que los dispositivos de John y Jane están bastante relacionados, por lo que se hablará de ellos aparte, pero haciendo menciones. En el ordenador de John, se han encontrado búsquedas de **tutoriales de encriptar**, dando a entender que a lo mejor, se han encriptado archivos de alguna manera. También se ha encontrado el **mismo billete que tenía Steve** en su ordenador junto con una **confirmación de envio de paquete de 20 kg**. Se conoce, gracias al ordenador de Jane, que fue John quien le compró los billetes a Steve, y quien envió el paquete a 5 34 Hapua Street Remuera Auckland 1050 New Zealand. Se encontró un **excel que contenía a los clientes**. Estaba el nombre de Steve, y un envío de un peso de 15kg a Jake, por lo que se confirma que el paquete contenía drogas.También se ve a Jane, por lo que se intuye una **relación cercana por la poca cantidad** y el hecho de las imágenes de los niños.También da lugar a dudas el historial de Jane en el que pretendía **hacerse pasar por una desesperada por drogas**.También se encuentran imágenes del uso de un programa para ocultar secretos en imágenes por medio de un **programa de esteganografía**. También se encuentra una imagen de un sitio. El punto es que está igual marcado que la imagen del mapa que tenía Steve, en este caso, pone , “put the drugs here”. También se han encontrado posibles métodos de ocultación de drogas y de una calle en específico tomada con prisas.

En el ordenador de Jane, se han encontrado en un primer lugar imágenes de **advertencias de venta de drogas en zonas de colegio**. Y también se ven imágenes de una cámara , parecidas a una videollamada o un hackeo de la cámara.En el historial de Jane, como se mencionó antes, se ve como **busca parecer desesperada por drogas, o las sentencias por estar relacionada con ellas**. También se descargó un programa, **Quasarv1.3.0.0** que parece servir como troyano para acceder a las pulsaciones de teclado o incluso a la cámara. Se ve como puede ver los inicios de sesión y conversaciones y contraseñas del **ordenador de John.** Se confirma que fue él quien le compró los billetes a Steve y parece ser quien maneja todo, por la lista de excel y Jane parece ser una ayudante. Se encontraron contraseñas para archivos de Attachments (Contraseña: ilovediving), una descarga desde la aplicación de esteganografía que la imagen descargada se llama BNE, como la que tiene Steve en su ordenador gracias a FTK,y la búsqueda de métodos de encriptación.Y también un archivo usado para la **ocultación de secretos**. Y se ve como John ha usado una app llamada **image steganography. Y que desde esa aplicación descargó una imagen que guardó como BNE en el ordenador de John, es decir , la que tiene Steve.** La contraseña para descifrar el secreto oculto en la imagen es Elchapo2. Se ve también un punto de recogida. Aunque también cabe la posiblidad de que Jane sea una agente encubierta que busque activamente verndedores de droga, por las imagenes de placas de policia encntrados en su PC.

Todo junto establece a **John como el vendedor** y a **Steve o a Jane como los compradores**, aunque parece que al menos Jane es policía encubierta. Jane podria ser tambien una "compradora" , aunque sea su papel ,por el hecho de que ha comprado algo a John, pero el hecho de que ha accedido a las pulsaciones de teclado de Steve, la poca cantidad de mercancía que pedía y el hecho de que no ponga en el excel que se hace mensualmente la entrega,la presencia del historial extraño que tiene y la imagen de sus hijos, puede dar a entender otras motivaciones de Jane, pero se debe seguir sospechando de ella ya que se la ha arrestado, puediendo indicsar comportamiento anómalo de su parte. Principalmente por el hecho de la sospecha de la cercanía de los 2 por haber viajado juntos o que john tenga supuestas imágenes de los hijos de Jane, lo que, junto con la idea de pretender verse desesperada por consumir sacada del historial, puede que haya habido problemas con los hijos de jane, los verdaderos, ya que los de la imagen pueden ser parte del papel que parece llevar a cabo,y la venta de drogas de John. Aunque el hecho de encontrar Attachments, important crucial to our method, el hecho de que sea our (Nuestro) puede entender que es más de uno.

Un punto a recalcar es la veracidad de las imágenes de los hijos de Jane, ya que , a lo mejor está en el papel de parecer una adicta a las drogas, como indica su historial, y lo haya enviado para engañar a John. 

Tras un analisis de todo lo recopilado la hipótesis mas fuerte es que John es el vendedor de drogas y Jane es una policia encubierta o una persona que tiene motivos de venganza contra John. Steve puede ser otro policia encubierto o un drogadicto auténtico pero colaborativo con las autoridades. Jane y Steve se pusieron en contacto con John para encontrarse y comprarle drogas. Jane incitó a John a descargar varios archivos, resultando que la contact card tenga el RAT Quasar con el que Jane espia a John. Pero Jane y John fueron arrestados en el aereopuerto. John negandose a colaborar y Jane parece insistente en ir a cierto sitio, la biblioteca.

# TEST PLAN {##-test-plan}

Antes de nada, hay que tener en cuenta ciertos derechos a la privacidad, que en estos casos son muy fácilmente infringidos por los investigadores ya que están buscando en el dispositivo de otra persona y podrían infringir estos derechos llevando a problemas legales por lo que en la investigación forense no se debe investigar lo que pueda llevar a otros casos, solo lo prioritario. En esta situación, en el ordenador de Steve, se deben buscar imágenes, mensajes, búsquedas de internet, descargas, etc., que relacionen a Steve con el tráfico de drogas. El uso de cualquier otra imagen que no sea relevante para la investigación en el informe o como evidencia implicaría problemas legales, incluso si el investigado es un criminal. Siendo así que existen leyes de protección de datos personales, y que, por lo general, se debería minimizar la exposición de la información personal del criminal ,no relevante, en el informe.

## Pasos para Test plan eficiente {###-pasos-para-test-plan-eficiente}

Para llevar a cabo un test plan eficiente, hay que tener una planificación previa antes de llevar a cabo la investigación:

1. **Definir el alcance de la investigación**: Planificación basada ante las necesidades de la investigación que se va a llevar a cabo, en este caso, lo que se espera encontrar o lo que se va a buscar.  
2. **Determinar una estrategia**: Definir qué métodos o pruebas se van a usar para definir el alcance y lograrlo o que hacer en caso de que pasen algunas situaciones u otras..  
3. **Determinar niveles/ Tipos de pruebas o procesos**: Determinar los tipos de pruebas que se van a llevar a cabo en la investigación.  
4. **Identificar herramientas**: Se necesitan conocer diversas herramientas antes de llevar a cabo el proyecto para tener en consideración el análisis, las comparaciones, el reporte del caso, el aseguramiento de que la información no ha sido alterada(en este caso)

(Bureau, s.f.)  
Para llevar a cabo un test plan efectivo, hay que tener en cuenta unos requisitos previos:

- Tener en consideración el sistema operativo de la evidencia  
- Tener en consideración también, varios campos como mensajes(Gmail , mensajes directos, etc) ,memoria (volátil y no volátil), etc. 
- Hay que tener en cuenta también el tiempo dado para el análisis, de esta manera, se puede organizar al grupo de manera efectiva en el tiempo dado  
- Hay que desarrollar un diagrama de flujo, siendo este un método de organización de pasos y caminos separados en base a lo que pueda ocurrir en la investigación. Esto es útil ya que no se pierde tiempo en pensar cuál va a ser el siguiente paso si algo falla o no. Este punto viene siendo el mismo que el de determinar niveles y procesos de la planificación previa explicada antes

(Martínez, 2024)

## Poner los pasos en práctica {###-poner-los-pasos-en-práctica}

El primer punto a tener en cuenta es la formación de equipo de profesionales para llevar a cabo el caso. Lo ideal sería que se formen subgrupos de 2-3 personas enfocadas en el  mismo ámbito de la investigación, dando como resultado un grupo de unas 8-9 personas, para que en la investigación puedan contrastar conclusiones, alternar el trabajo u organizarlo de manera efectiva ya sea que un grupo se encargue de la recolección de las evidencias físicas y que se encargue del volcado de memoria y que se asegure de mantener intactas las evidencias o recopilando la información mientras otro busca evidencias en la memoria usando las herramientas respectivas.  
En el caso dado ,se espera encontrar cualquier tipo de evidencia(Ya sean imágenes , mensajes, o alguna otra pista que conduzca a una evidencia válida) que incrimine a Steve, el dueño del ordenador encontrado.

- **Definir el alcance**: Siendo el objetivo que el grupo encuentre evidencias que involucren a Steve con el tráfico de drogas, se espera encontrar imágenes que lo relacionen con esto, es decir, que el alcance de la investigación llega hasta algo que lo relacione con tráfico de drogas, más allá ya estaríamos sobrepasando dicho alcance y , tal vez, infringiendo algún derecho.  
- **Determinar una estrategia**: La estrategia a seguir , se verá en el diagrama  
- **Determinar niveles/Pruebas/Procesos**: En esta sección, se deben hacer pruebas y procedimientos para asegurar la integridad de los datos originales, para saber que ningún archivo ha sido alterado, determinar procesos para analizar el dispositivo,o para la adquisición de evidencias del mismo, etc.  
- **Herramientas**: Las herramientas que se van a usar es una indicación útil para esta situación , ya que se necesitan pruebas en tiempo real, no basta con imágenes, los informes son principalmente informativos y las herramientas se usan para la comprobación de las evidencias.Las herramientas usadas son:  
  - Autopsy: Para el análisis de las evidencias  
  - FTK Imager: Para la recolección de evidencias, y en parte también puede servir para el análisis de las evidencias si se ve desde otro punto de vista  
  - Volatility:Para el análisis de evidencias en la memoria RAM  
  - OpenStego: Para la recolección evidencias (de secretos en imágenes u otros archivos)

Una vez terminado se debe revisar que la memoria no ha sido alterada, usando hashmyfiles, si ha cambiado algún hash, significa que ha habido algún cambio en la memoria y se debería de “volver a empezar” (ya se saben donde hay evidencias).

## Diagrama {###-diagrama}

![img79](img/img79.png) 

## Buenas prácticas {###-buenas-prácticas}

### Prácticas para toda investigación {####-prácticas-para-toda-investigación}

Las prácticas básicas, y generales, para esta y cualquier investigación forense (en un contexto similar) serían:

* Usar un entorno controlado: Esto se debe a que es posible que se produzcan errores o que al exportar algún tipo de evidencia cause problemas en nuestro dispositivo de análisis principal. Una máquina virtual bien implementada debería servir para exportar evidencias sin miedo a errores en nuestro dispositivo.  
* Mantener la integridad de la memoria: Esto se puede hacer con herramientas como Hashmyfiles, que nos dan hashes que nos informarán si ha habido cambios de algún tipo en la memoria. Si la evidencia original se altera, cabe la posibilidad de que las rutas o procedimientos o incluso perder evidencias, ya que las imágenes que se toman durante la investigación no se pueden considerar como tal.  
* Mantener el equipo de las evidencias intacto: Si a este equipo le ocurre cualquier alteración, las evidencias perderían credibilidad y no serían útiles en el caso, o no del todo al menos. No será necesario encenderlo ni conectarlo a ninguna red de internet debido a los riesgos que puede implicar

### Prácticas para este caso específico {####-prácticas-para-este-caso-específico}

Ahora las recomendaciones para este caso específico:

- Usar alguna otra herramienta si se cree necesario: No hay que regirse solo a las herramientas que tenemos en un principio, si descubrimos algo con lo que haya que usar alguna otra herramienta que debamos descargar, lo probamos, con el fin de ayudar en la investigación  
- Comparar las imágenes encontradas en FTK Imager con autopsy, o viceversa, para confirmar información, no contrastada ya que no son exactamente herramientas de forense que se usen para contrastar información entre ellas, pero se puede usar para sacar conclusiones o saber que se hizo con diferentes archivos  
- Recolectar toda la evidencia que se crea importante. En una investigación nos debemos centrar en lo que se nos manda buscar en un dispositivo, la evidencia que no tenga que ver con el caso no solo es inservible, sino que también podemos meternos en problemas legales respecto a la privacidadc

Las buenas prácticas son normalmente recomendaciones que se deberían de seguir en todas las investigaciones forenses:

- Tomar capturas de pantalla adecuadas del sistema y de su análisis(RFC 3227): Esta práctica sirve para hacer de guía, ya que las tomas de captura de pantalla no sirven como evidencia valida en un caso real, sino más bien para indicar adónde ir o qué se espera encontrar al llevar a cabo ciertas acciones, desde la experiencia  
- Mantener notas detalladas en todo momento de lo que se hace o de lo que pasa con el sistema por si en el futuro se requieren para un análisis(RFC 3227): Junto con el anterior punto, el hecho de crear notas detalladas para mostrar paso a paso lo que se hace o se deja de hacer para llegar a las videncias. Hay que hacerlo con el objetivo de que gente que no sea experta en análisis forenses pueda llegar a las mismas conclusiones a las que yo he llegado.  
- Tener en consideración la hora del equipo analizado y el propio(RFC 3227): Sirve para validad aun más las evidencias, ya que si no se tiene en cuenta, las evidencias encontradas podrían acabar siendo consideradas como inválidas en el caso  
- Minimizar los cambios en los datos a la hora de exportar archivos, básicamente mantener la integridad de la evidencia original(RFC 3227): Si la evidencia original cambia, se podrían perder evidencias que puedan ser útiles para la investigación, o estas pruebas también podrían volverse inaccesibles   
- Primero se debería llevar a cabo la recolección y después el análisis de las evidencias(RFC 3227): Una vez las evidencias recolectadas, la evidencia original se puede poner en cuarentena para evitar cambios en ella y evitar cambios inesperados en la evidencia original. 

(Brezinski, 2002)

- Mantener los datos originales intactos , ya sea una memoria de reserva o el propio dispositivo analizado ya que se puede corromper, alterar, etc.  
- Mantener la claridad en la investigación, sin incluir datos no relevantes o que puedan llevar a malentendidos de diversos tipos. En una investigación se debe buscar lo que se pide, por una parte, para no perder tiempo, por otra parte, para evitar infringir derechos de la privacidad

(Martínez, 2024)  
Como se ve en los paréntesis, se mencionan principalmente recomendaciones de una norma en específico, la RFC 3227.Esto es un documento en el que se recogen las directrices para la recopilación de evidencias y su almacenamiento, pudiendo llegar a ser un estándar estándar para la recopilación de la información o de evidencias,.  
(Incibe, s.f.)  
El cumplimiento de las buenas practicas es una recomendación, en un primer lugar, pero también ayudan con los procesos legales y éticos:

- Cadena de custodia: La buena documentación de las evidencias minimiza el riesgo de perderlas o de que un juez no pueda acceder a ellas.  
- Veracidad de las evidencias frente a un juicio: Siguiendo el punto anterior, la evidencia se debe documentar de manera correcta para que un juez, o cualquier otra persona pueda llegara a las evidencias con las indicaciones. Pero , la evidencia original se debe mantener intacta para que se pueda volver a acceder a ella.

El punto de usar buenas practicas en las investigaciones está en que ayudan a llevar cierto orden o saber lo que hacer, básicamente para evitar errores, o fallos inesperados. Esto también aplica a la veracidad de las pruebas y evidencias, si se aplican buenas prácticas, podemos asegurar, en cierta manera, la veracidad de estas y tener un punto de apoyo más en el caso. En este caso, el uso de buenas prácticas como en el mantener las evidencias originales intactas o tener menos riesgos a la hora de analiza respecto a los marcos legales o incluso los éticos ya que estos van bastante a la par , al menos bajo mi punto de vista. El no implementar las buenas prácticas, o implementarlas erróneamente puede llevar a problemas legales, como ya se mencionó, o las evidencias podrían perder veracidad al no llevar a cabo buenas prácticas.

## Evaluación crítica personal {##-evaluación-crítica-personal}

Evaluación crítica personal de la investigación forense digital:

- Se debería haber tomado más imágenes para mostrar todo lo que es relevante, y se debería de haber dejado de lado algunas imágenes que podrían comprometer la privacidad del investigado.  
- Se debería de haber sido más específico con las rutas y procedimientos seguidos.  
- Estar más abierto al uso de otras herramientas es esencial para mejorar la calidad del informe y de la investigación inicial, y junto a esto, haber pensado en varias posibilidades a la hora de establecer las herramientas habría ayudado a una mejor investigación desde un principio  
- Se ha mencionado información en el informe que no es del todo relevante en la investigación, y que es más personal a pesar de no haber sacado captura de ellas

# Bibliografía {##-bibliografía}

Brezinski, D. &. K., 2002. *RFC 3227.* [En línea]   
Available at: https://www.rfc-editor.org/rfc/rfc3227#section-2  
[Último acceso: 14 11 2024].  
Bureau, S. T., s.f. *Crear un buen Plan de Pruebas. Software Testing Bureau.* [En línea]   
Available at: https://www.softwaretestingbureau.com/crear-un-buenplan-de-pruebas/   
[Último acceso: 14 11 2024].  
Duriva, 2023. *Desafíos Éticos en el Peritaje Informático.* [En línea]   
Available at: https://duriva.com/desafios-eticos-en-el-peritaje-informatico/  
[Último acceso: 12 2 2025].  
europea, P. E. y. e. c. d. l. u., 2016. *REGLAMENTO (UE) 2016/679.* [En línea]   
Available at: https://www.boe.es/doue/2016/119/L00001-00088.pdf  
[Último acceso: 7 2 2025].  
Explorer, U., s.f. *Los sistemas de archivos de Windows.* [En línea]   
Available at: https://www.ufsexplorer.com/es/articles/windows-file-systems/?srsltid=AfmBOooYr4gs80yi7ArLOVFakG57CHiwHrqqhrw7Jz1Xdxr1M4YYR8Iq  
[Último acceso: 10 2 2025].  
Gonzalez, Á., 2015. *ISO/IEC 27042:2015: Garantizando la Integridad del Análisis de Evidencias Digitales en Procesos Judiciales.* [En línea]   
Available at: https://peritosinformaticos.es/iso-27042-perito-informatico/  
[Último acceso: 9 2 2025].  
Incibe, s.f. *RFC 3227- Directrices para la recopilación de evidencias y su almacenamiento.* [En línea]   
Available at: https://www.incibe.es/incibe-cert/blog/rfc3227  
[Último acceso: 10 1 2025].  
Interpol, s.f. *Analisis forense digital.* [En línea]   
Available at: https://www.interpol.int/es/Como-trabajamos/Innovacion/Analisis-forense-digital  
[Último acceso: 7 2 2024].  
Martínez, A., 2014. *RFC 3227 - Directrices para la recopilación de evidencias y su almacenamiento.* [En línea]   
Available at: https://www.incibe.es/incibe-cert/blog/rfc3227  
[Último acceso: 7 2 2025].  
Martínez, L., 2024. *LO2-Normativa.* [En línea]   
Available at: https://classroom.google.com/u/3/w/NzAyMjg4MjY1MTIz/t/all  
[Último acceso: 11 2 2025].  
Martínez, L., 2024. *LO3- Usar diferentes herramientas para realizar investigaciones forenses digitales en dispositivos o redes para investigar ataques cibernéticos.* [En línea]   
Available at: https://classroom.google.com/u/3/w/NzAyMjg4MjY1MTIz/t/all  
[Último acceso: 12 2 2025].  
Martínez, L., 2024. *LO4- Test Plan y buenas prácticas.* [En línea] 
Available at: https://classroom.google.com/u/3/c/NzAyMjg4MjY1MTIz/m/Njg2OTk3ODAwMjI1/details  
[Último acceso: 14 11 2024].  
Martinez, L., s.f. *LO1 Procesos y Procedimientos.* s.l.:s.n.  
Rafael, 2012. *ISO/IEC 27037:2012 Nueva norma para la Recopilación de Evidencias..* [En línea]   
Available at: https://peritoit.com/2012/10/23/isoiec-270372012-nueva-norma-para-la-recopilacion-de-evidencias/  
[Último acceso: 9 2 2025].
[Ch4mbi](https://github.com/Ch4mbi)
