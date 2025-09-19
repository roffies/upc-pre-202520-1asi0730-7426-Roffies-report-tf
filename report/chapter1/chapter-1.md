# **Capítulo I: Introducción**

## 1.1. Startup Profile
 En esta sección se presenta la descripción del startup y los perfiles de los miembros del equipo.

### 1.1.1. Descripción de la Startup
Roffies es una startup tecnológica enfocada en modernizar el mantenimiento automotriz en Lima y, progresivamente, en todo el país. Nuestro producto principal, SmartCare, es una plataforma web que centraliza la afiliación de talleres mecánicos (especializados por marca y generales) y conecta a dueños de vehículos con servicios confiables para programar citas, recibir alertas y cotizar trabajos en tiempo real.

La propuesta de valor de Roffies se basa en analizar el historial de vehículos, el kilometraje y la data técnica de fabricantes para estimar costos, sugerir servicios preventivos y anticipar necesidades antes de que se conviertan en averías. Con ello buscamos reducir gastos inesperados, mejorar la seguridad vial y aumentar la transparencia de precios y diagnósticos.

El sistema consiste en un historial digital de mantenimientos, alertas de mantenimiento basadas en datos por marca y uso, cotizador en tiempo real entre talleres afiliados, botón de pánico para averías en ruta, conexión directa con grúas y derivación automática al taller más cercano con disponibilidad. 

- **Misión:** transformar la experiencia de mantenimiento vehicular en el Perú mediante tecnología predictiva, datos confiables y una red de talleres de calidad, entregando al conductor control y tranquilidad, y al taller, eficiencia y clientes fieles.

- **Visión:** ser la plataforma líder a nivel nacional en servicios automotrices digitales, reconocida por prevenir averías, profesionalizar la relación taller–cliente y elevar el estándar del servicio mecánico en el Perú.


**Logotipo del servicio**
![MockupWebApp1](../../assets/SmartCare_logo.png)

### 1.1.2. Perfiles de integrantes del equipo

|                                             **Integrantes**                                              |                                                                                                                                                                                            **Descripción del Perfil**                                                                                                                                                                                            |
| :------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| **Piero Angel Sulca Sanchez(U202423711)**<br/><img src="../../assets/piero-sulca-sanchez.png" width="300"/> | <div align="justify">Me llamo Piero Angel Sulca Sanchez, soy estudiante de Ingeniería de Software. Me gusta trabajar en equipo pues me permite aprender sobre las ideas que tienen los participantes y contrastarlas con las mías para poder seguir mejorando. Tengo conocimiento en tecnologías de desarrollo web como TypeScript, React, Next.js y NestJS. Estoy muy interesado en el desarrollo de aplicaciones web.</div> |
|                     **Rúbens Bendezu Navarro (U20231d390)**<br/><img src="../../assets/profile_rubens_bendezu.jpeg" width="300"/>                     |          <div align="justify">Me llamo Rúbens Bendezu Navarro, soy estudiante de Ingeniería de Software. Me considero una persona motivada por el aprendizaje continuo y el trabajo en equipo, ya que compartir ideas y experiencias enriquece tanto el desarrollo personal como el profesional. Tengo conocimientos en tecnologías de desarrollo web y frameworks modernos, y me interesa especialmente el desarrollo de aplicaciones web que aporten soluciones innovadoras y de impacto.</div>                                                                                                                                                                                                                                                                                                                                                                                                         |
|                     **Luis Sebastián Rubio Ortiz (U202310349)**<br/><img src="../../assets/Luis Sebastián Rubio Ortiz.jpg" width="300"/>                     | <div align="justify">Me llamo Luis Sebastián Rubio ortiz, soy estudiante de Ingeniería de Software y actualmente estoy cursando el quinto ciclo. Considero que soy una persona responsable, me gusta aprender cosas nuevas constantemente y me gusta apoyar a mis compañeros con cualquier cosa que necesiten.</div> |
|                     **Johan Karl Bottger Salazar (u202210735)**<br/><img src="../../assets/Johan.jpg" width="300"/>                     |  <div align="justify">Soy Johan Karl Bottger Salazar, y soy estudiante de Ingeniería de Software. Tengo mucho interés en las metodologías ágiles y me gustaría especializarme en ello.</div>                                                                                                                                                                                                                                                                                                                                                                                                                |
|                     **Pierina Marysabel Almandroz Carbajal (U202316845)**<br/><img src="../../assets/Pierina_Almandroz_Carbajal.jpeg" width="300"/>                     |  Soy Pierina, tengo 19 años, soy estudiante de 5to ciclo de Ing. de Software. Me encuentro comprometida con el grupo y tengo un gran interés en el desarrollo de aplicaciones web, área en la que busco seguir especializándome.                                                                                                                                                                                                                                                                                                                                                                                                                |


## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

Lima concentra una porción significativa del parque automotor del país y la demanda por servicios de mantenimiento crece de forma sostenida. La Asociación Automotriz del Perú (AAP) difunde mensualmente estadísticas del sector, mostrando evolución de ventas e inmatriculaciones, un contexto que empuja la necesidad de profesionalizar y digitalizar la posventa (mecánica, repuestos, auxilio) 
Por otro lado, la seguridad vial y la atención de emergencias son temas críticos: el Observatorio Nacional de Seguridad Vial reportó en 2023 más de 87 mil siniestros, con miles de personas lesionadas o fallecidas; ello refuerza la importancia de un botón de auxilio y derivación rápida a grúa y taller.

**What**
**¿Cuál es el problema?**
Los conductores carecen de una plataforma confiable y transparente para gestionar el mantenimiento de su vehículo, comparar precios, registrar historial y recibir alertas preventivas; los talleres, a su vez, no cuentan con herramientas estandarizadas para captar y fidelizar clientes con métricas de calidad.

**When**
**¿Cuándo sucede el problema?**
Durante todo el ciclo de vida del vehículo: mantenimientos preventivos por kilometraje/tiempo, reparaciones correctivas, pre–ITV, y emergencias en ruta.

**Where**
**¿Dónde surge el problema?**
Inicialmente en Lima Metropolitana, con expansión nacional planificada a partir de tracción en ejes urbanos regionales.

**Who**
**¿Quiénes están involucrados? ¿Quién lo utilizará?**
Conductores de autos particulares y pequeñas flotas, talleres mecánicos afiliados (generales y especialistas), empresas de grúas y, como aliados, aseguradoras y distribuidores de repuestos.

**Why**
**¿Por qué? ¿Cuál es la causa del problema?**
Informalidad y heterogeneidad de estándares de servicio, ausencia de historial centralizado, baja transparencia de precios y escaso uso de datos para la prevención.

**¿Cuáles son las 2H?**

**How (Cómo)**
**¿Cómo se utilizará el producto?**
El conductor registra su vehículo, recibe alertas de mantenimiento, cotiza y agenda con talleres verificados; el taller gestiona disponibilidad, precios, reputación y reporta trabajos a un historial único. En emergencias, el usuario activa SOS para conexión inmediata con grúa y derivación al taller más cercano disponible.

**How much (Cuánto)**
**¿Cuál es la magnitud del problema?**
El tamaño del mercado puede inferirse por la masa vehicular y su gasto recurrente en mantenimiento y reparación; la publicación periódica de la AAP sobre ventas y el crecimiento de líneas móviles sugieren condiciones atractivas para una plataforma de servicios posventa escalable.


## 1.2.2. Lean UX Process

### 1.2.2.1. Lean UX Problem Statements

**Problem Statement**

En Lima, los conductores enfrentan una constante incertidumbre respecto al cuidado de sus vehículos. No cuentan con información clara ni centralizada sobre qué mantenimiento requiere su auto, en qué momento debe realizarlo ni cuánto debería costar. En la práctica, la mayoría elige talleres en función de la cercanía geográfica o recomendaciones informales, lo que los expone a diagnósticos poco transparentes, precios dispares e incluso a reparaciones innecesarias. Esta falta de estandarización deriva en averías que podrían haberse prevenido, incrementando los riesgos de seguridad en ruta y generando gastos inesperados que afectan directamente al bolsillo del usuario.

Del otro lado, los talleres mecánicos, especialmente los independientes, carecen de herramientas digitales que les permitan diferenciarse en un mercado cada vez más competitivo. Muchos no pueden visibilizar adecuadamente su propuesta de valor, gestionar agendas de manera eficiente ni consolidar una reputación verificable basada en la experiencia real de los clientes. Como resultado, pierden oportunidades de fidelización y de captar nuevos usuarios que buscan confianza y profesionalismo.

Esta brecha estructural entre oferta y demanda, sin un historial único del vehículo ni alertas de mantenimiento basadas en datos concretos; genera sobrecostos, tiempos muertos y pérdidas de productividad para los usuarios. Al mismo tiempo, limita el crecimiento y formalización de los talleres, perpetuando un ecosistema fragmentado, poco transparente y vulnerable a la desconfianza. Resolver esta problemática no solo representa una oportunidad de innovación tecnológica, sino también una contribución a la seguridad vial y a la modernización del sector automotriz en el Perú.


### 1.2.2.2. Lean UX Assumptions

**Business Assumptions**

- Creemos que nuestros usuarios necesitan una forma más confiable, rápida y basada en datos para conectar sus vehículos privados con talleres mecánicos especializados y generales.
- Estas necesidades pueden satisfacerse con una plataforma web que afilie talleres confiables, gestione historiales digitales y emita alertas predictivas de mantenimiento.
- Nuestros primeros clientes serán propietarios de vehículos privados en Lima Metropolitana que buscan conservar sus autos en buen estado y acceder a precios transparentes.
- El valor más importante que un cliente quiere es llevar el historial de su vehículo, recibir alertas de mantenimiento, comparar precios en tiempo real y contar con un botón de pánico en emergencias.
- Los clientes también obtendrán tranquilidad por tener sus datos centralizados y los talleres ganarán visibilidad digital y más clientes.
- Vamos a adquirir la mayoría de clientes mediante alianzas estratégicas, marketing digital y colaboraciones con aseguradoras y empresas de movilidad.
- Obtendremos ingresos por comisión en transacciones, suscripciones premium para talleres y márgenes en un marketplace de productos automotrices.
- Nuestra competencia directa incluye aplicaciones de aseguradoras y directorios en línea, pero ninguno ofrece un ecosistema integral con historial digital y predictor inteligente.
- Nuestra ventaja competitiva es que Roffies no solo conecta talleres y conductores, sino que ofrece un sistema integral con datos predictivos, historial exclusivo y soporte en emergencias.
  
- El mayor riesgo es que talleres tradicionales no adopten la herramienta y que conductores desconfíen de los talleres afiliados al inicio.
- Este riesgo se mitigará con una interfaz amigable, procesos claros y casos de éxito que validen los resultados.

**User Assumptions**

**¿Quién es el usuario?**

Nuestros usuarios principales son los dueños de vehículos particulares que circulan en Lima Metropolitana y desean una forma práctica de cuidar su vehículo sin gastar de más. En paralelo, los talleres mecánicos afiliados son usuarios claves de la plataforma, ya que gestionarán su reputación, agenda y relación con clientes a través de Roffies.

**¿Qué problemas tiene nuestro usuario que el producto debe resolver?**

- Los conductores enfrentan dificultad para encontrar talleres confiables y no tienen una forma estandarizada de comparar precios y servicios.
- Carecen de un historial centralizado que muestre mantenimientos pasados, lo que genera diagnósticos poco precisos y repetición de trabajos.
- Están expuestos a averías en ruta por no contar con alertas de mantenimiento preventivo.
- Los talleres, en cambio, tienen problemas para captar clientes en un mercado saturado, no cuentan con herramientas de visibilidad digital ni sistemas modernos de gestión.

**¿Qué características son importantes?**

Los usuarios valoran funcionalidades como:

- Registro del vehículo y mantenimiento de un historial digitalizado.
- Alertas predictivas basadas en kilometraje y datos de fabricantes.
- Cotizador en tiempo real con comparación entre talleres afiliados.
- Botón de emergencia para asistencia en ruta.
- Agenda online y pago digital seguro.
- Reputación verificable de talleres basada en reseñas de clientes y métricas de desempeño.


**¿Dónde encaja el producto en su trabajo o vida diaria?**

La plataforma se convierte en parte de la rutina de gestión del vehículo. Para los conductores, Roffies actúa como un “asistente digital automotriz” que les recuerda cuándo y dónde realizar mantenimientos. Para talleres, se integra como su agenda principal de gestión, reemplazando procesos manuales de registro de citas.

**¿Cuándo y cómo se usará el producto?**

El producto se usará en distintos momentos críticos:
- Antes de un mantenimiento programado, cuando la plataforma envía alertas predictivas.
- Durante la comparación de precios, cuando el conductor busca transparencia y ahorro.
- En emergencias, con el uso del botón de pánico y la conexión con grúa.
- En la administración diaria de talleres, al gestionar clientes, citas y métricas.

**¿Cómo debe verse y comportarse el producto?**

Debe tener una interfaz moderna, confiable e intuitiva, diseñada para un público amplio, desde jóvenes usuarios digitales hasta conductores de mayor edad. La experiencia debe transmitir seguridad, simplicidad y transparencia. El sistema debe proteger datos sensibles, garantizar disponibilidad 24/7 y permitir personalización de acuerdo al perfil del usuario (conductor o taller).

**Future Assumptions** 

- **Creemos que** la plataforma debe evolucionar hacia la integración con IoT y telemática, permitiendo que los vehículos conectados envíen datos automáticos a Roffies para generar alertas sin intervención manual.
- **Creemos que** debe incluir inteligencia artificial para sugerir mantenimientos no solo basados en kilometraje, sino también en patrones de uso y estilo de conducción.
- **Creemos que** debe contar con un sistema de reputación sólido para talleres, con badges de calidad y certificaciones verificables.
- **Creemos que** debe integrarse con aseguradoras para ofrecer seguros personalizados según historial de mantenimiento.
- **Creemos que** debe tener dashboards visuales de métricas para conductores (ahorro, historial, proyecciones) y para talleres (clientes atendidos, ingresos, eficiencia).
- **Creemos que** a futuro se expandirá con servicios adicionales: compra-venta de vehículos usados con historial certificado, financiamiento de reparaciones y alianzas con fabricantes para garantías extendidas.

---

### 1.2.2.3. Lean UX Hypothesis Statements

#### Hypothesis Statement 01

Creemos que los conductores en Lima Metropolitana estarán dispuestos a registrar sus vehículos en Roffies para recibir alertas de mantenimiento predictivas, historial digital y cotizaciones claras entre talleres afiliados.

Sabremos que hemos tenido éxito

Cuando al menos el 60 % de los usuarios que descarguen la aplicación completen el registro de su vehículo y generen al menos una cotización en los primeros 15 días de uso.



#### Hypothesis Statement 02

Creemos que los talleres mecánicos (especializados y generales) estarán interesados en afiliarse a Roffies para aumentar su visibilidad digital, captar clientes nuevos y mejorar su reputación con reseñas verificadas.

Sabremos que hemos tenido éxito

Cuando al menos el 40 % de los talleres afiliados reciban cinco o más reservas mensuales en los primeros tres meses de uso de la plataforma.



#### Hypothesis Statement 03

Creemos que la integración del botón de emergencia (SOS) que conecta al conductor con grúas y talleres cercanos incrementará significativamente la confianza y satisfacción de los usuarios.

Sabremos que hemos tenido éxito

Cuando al menos el 30 % de los conductores activos utilice el botón SOS al menos una vez durante el primer año y reportan una satisfacción superior al 70 % en encuestas posteriores al servicio.


#### Hypothesis Statement 04

Creemos que el predictor de mantenimiento reducirá las averías correctivas inesperadas al anticipar servicios preventivos basados en historial y kilometraje.

Sabremos que hemos tenido éxito

Cuando al menos el 25 % de los conductores que utilicen la función de alertas predictivas registran una reducción en sus averías correctivas en un periodo de seis meses, en comparación con usuarios que no activen esta función.



#### 1.2.2.4. Lean UX Canvas

| Business Problem | Solution Ideas | Business Outcomes |
|------------------|----------------|-------------------|
| En Lima, los conductores carecen de una plataforma confiable y centralizada para gestionar el mantenimiento de sus autos. La mayoría depende de talleres informales, recomendaciones de boca a boca o búsquedas poco estructuradas en internet, lo que genera falta de transparencia en precios, ausencia de historial de mantenimientos y averías inesperadas.<br><br>Por el lado de los talleres, no existen canales digitales estandarizados para captar clientes, diferenciarse en un mercado saturado ni administrar de manera profesional citas y reputación. | ● Aplicación web y móvil que centraliza registro de vehículos, agenda y cotización de mantenimientos.<br>● Predictor inteligente que analiza historial, kilometraje y data de fabricantes para anticipar servicios.<br>● Cotizador en tiempo real para comparar precios y tiempos de talleres afiliados.<br>● Botón de pánico (SOS) con conexión a grúa y talleres cercanos.<br>● Marketplace de repuestos y consumibles automotrices.<br>● Sistema de reputación y certificación de talleres basado en reseñas verificadas y métricas de calidad. | ● Alcanzar 5,000 conductores registrados y 300 talleres afiliados en Lima en el primer año.<br>● Lograr que el 50 % de los talleres afiliados reciban al menos cinco citas mensuales en los primeros seis meses.<br>● Reducir en un 20 % las averías correctivas reportadas por conductores que utilizan alertas predictivas durante los primeros seis meses.<br>● Obtener un Net Promoter Score (NPS) superior a 60 en los usuarios que usen el botón de emergencia (SOS).<br>● Generar ingresos sostenibles mediante comisiones por servicios, suscripciones premium de talleres y ventas en el marketplace automotriz. |
| Hypotheses | Users & Customers | User Benefits |
| ● Los conductores adoptarán Roffies si perciben ahorro en tiempo y dinero mediante cotizaciones claras y recordatorios automáticos.<br>● Talleres evaluarán si ven un incremento rápido en reservas y reputación digital.<br>● El botón de emergencia será clave para fidelizar a usuarios que valoren asistencia rápida.<br>● El predictor de mantenimiento reducirá averías correctivas, mejorando satisfacción y confianza.<br>● Integrar repuestos en el marketplace generará recurrencia y fortalecerá la relación usuario–taller. | ● Conductores particulares: personas que buscan confianza, transparencia y seguridad al mantener su vehículo.<br>● Administradores de flotas pequeñas: taxis, aplicaciones de movilidad y empresas de reparto que requieren control de costos y disponibilidad de sus unidades.<br>● Talleres mecánicos: generales e independientes que desean captar clientes y profesionalizar su gestión.<br>● Aliados estratégicos: aseguradoras, grúas y proveedores de repuestos que se integran al ecosistema. | ● Para conductores: historial digital unificado, alertas predictivas de mantenimiento, cotizaciones transparentes y soporte inmediato en emergencias.<br>● Para talleres: más visibilidad en un mercado competitivo, flujo constante de clientes, herramientas de gestión de citas y métricas de reputación.<br>● Para aliados: un nuevo canal de venta y fidelización integrado a un ecosistema digital. |
| What’s the most important thing we need to learn first? | What’s the least amount of work we need to do to learn the next most important thing? |
| Necesitamos validar si los conductores realmente están dispuestos a registrar su vehículo y confiar en cotizaciones comparativas entre talleres. También debemos aprender qué factores (precio, cercanía, reputación, rapidez) pesan más en la decisión de contratar un servicio. | ● Construir un MVP en dos distritos de Lima con 15–20 talleres afiliados y 200–300 conductores.<br>● Incluir tres funciones básicas: registro de vehículo, cotización comparativa y agenda de citas.<br>● Medir adopción inicial, tasa de conversión de cotización a reserva y feedback de confianza en el proceso.<br>● Ajustar la propuesta antes de ampliar a más distritos y funciones avanzadas (alertas predictivas, SOS, marketplace). |

## 1.3. Segmentos objetivos.
**Conductores de vehículos particulares**

Este segmento incluye a propietarios de automóviles particulares. De acuerdo con la Asociación Automotriz del Perú (AAP), en 2023 el parque automotor peruano superó los 3,5 millones de vehículos, de los cuales más del 65 % se concentran en Lima y Callao (AAP, 2023). Este crecimiento constante genera una demanda creciente de servicios de mantenimiento y reparación. Sin embargo, los conductores enfrentan problemas de informalidad en talleres, sobrecostos y ausencia de historiales de servicio digitalizados, lo que afecta la seguridad y la eficiencia del uso de sus vehículos.
Para este grupo, Roffies ofrece beneficios como la centralización del historial de mantenimientos, alertas predictivas basadas en kilometraje y data de fabricantes, cotizaciones transparentes entre talleres y un botón de emergencia para asistencia inmediata en ruta. Estos atributos incrementan la confianza, reducen costos imprevistos y mejoran la seguridad vial en una ciudad con altos índices de congestión y accidentes.


**Talleres mecánicos afiliados (generales y especializados)**

El segundo segmento lo conforman talleres mecánicos independientes y especializados que operan en Lima Metropolitana. Según datos del Instituto Nacional de Estadística e Informática (INEI), más del 70 % de los talleres automotrices en el Perú son micro y pequeñas empresas (MYPEs), con un alto nivel de informalidad y escasa digitalización (INEI, 2022). La mayoría carece de herramientas tecnológicas para gestionar clientes, mejorar su reputación y competir en un mercado cada vez más exigente.
Para los talleres, Roffies representa una oportunidad de transformación digital: visibilidad en un marketplace confiable, captación de clientes nuevos sin altos costos de publicidad, sistema de reputación con reseñas verificadas y herramientas para gestionar agendas y métricas de desempeño. Al integrarse en la plataforma, los talleres pueden diferenciarse de la competencia, fidelizar clientes y aumentar sus ingresos.