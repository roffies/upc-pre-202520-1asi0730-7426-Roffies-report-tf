# Capítulo III: Requirements Specification
En este capítulo se especifican los requisitos del MVP de **SmartCare**, definidos a partir del análisis de usuarios, entrevistas y artefactos de investigación realizados previamente. El alcance se centra en dos funcionalidades principales: la gestión del historial digital de mantenimientos y el predictor de servicios y costos, que responden directamente a las necesidades identificadas en los segmentos objetivo (dueños de vehículo y dueños de talleres).  

Asimismo, se incluyen historias de negocio, técnicas y de soporte (Landing Page), necesarias para garantizar la operatividad, escalabilidad y valor integral del sistema.

## 3.1. To-Be Scenario Mapping
El mapeo de escenarios *To-Be* permite visualizar el flujo de trabajo deseado en el futuro, una vez implementadas las mejoras propuestas con **SmartCare**. Estos escenarios se construyeron en base a la investigación previa y muestran cómo la plataforma transformará la experiencia de los dueños de vehículo y talleres.  

Al compararlos con los escenarios actuales (*As-Is*), se identifican los cambios clave que introducirá nuestra solución: mayor trazabilidad del historial, predicciones de mantenimiento confiables y comunicación más transparente entre usuarios y talleres.  

A continuación, se presentan los escenarios *To-Be* para nuestros dos segmentos objetivos principales.

**To-Be Scenario: Segmento Objetivo - Dueño de vehículo**

![To-Be Scenario Mapping Conductor](../../assets/31-to-be-scenario-mapping-conductor.jpg)

**To-Be Scenario: Segmento Objetivo - Jefe/Asesor de Taller Afiliado**

![To-Be Scenario Mapping Jefe Taller](../../assets/31-to-be-scenario-mapping-jefe-taller.jpg)

## 3.2. User Stories 
Las User Stories se redactaron a partir de las necesidades identificadas en la investigación previa, considerando los segmentos objetivo (dueños de vehículos y dueños de talleres). Además, se incluyen historias de negocio, técnicas y de soporte (Landing Page), que son necesarias para asegurar la correcta operación y adopción de **SmartCare**.

A continuación se presentan las epicas formuladas para elaborar las *User Stories*.

# Tabla de Épicas

| Epic ID | Título | Descripción |
| --- | --- | --- |
| EP01 | Cuentas y Acceso | **Como** usuario, **quiero** crear, autenticar y gestionar mi perfil **para** acceder de manera segura y personalizada a la plataforma. |
| EP02 | Vehículo e Historial Digital | **Como** dueño de vehículo, **quiero** registrar mis vehículos y consolidar su historial digital de mantenimiento **para** tener control y trazabilidad de todos los servicios realizados. |
| EP03 | Agenda y Citas | **Como** dueño de vehículo, **quiero** buscar talleres y gestionar mis citas (reserva, reprogramación, cancelación) **para** asegurar la atención de mi vehículo de forma conveniente. |
| EP04 | Gestión de Taller y Órdenes de Trabajo | **Como** jefe o asesor de taller, **quiero** administrar el perfil, la agenda y las órdenes de trabajo **para** organizar mejor mis operaciones y generar confianza en mis clientes. |
| EP05 | Predictor y Recomendaciones | **Como** dueño de vehículo, **quiero** recibir predicciones de mantenimiento basadas en historial, pautas y uso del vehículo **para** anticipar costos y prevenir averías. |
| EP06 | Comunicaciones y Notificaciones | **Como** usuario, **quiero** recibir correos y notificaciones transaccionales **para** estar informado oportunamente sobre mis citas y servicios. |
| EP07 | Catálogo y Datos Maestros | **Como** administrador, **quiero** gestionar tipos de servicio y pautas de fabricante **para** asegurar la consistencia de los datos y el correcto funcionamiento del predictor. |
| EP08 | Landing Page y Adquisición | **Como** visitante, **quiero** conocer la propuesta de valor y beneficios de la plataforma **para** decidir registrarme o afiliar mi taller. |
| EP09 | Arquitectura y Tareas Técnicas | **Como** desarrollador, **quiero** implementar tareas técnicas y configurar la arquitectura **para** garantizar la operatividad, seguridad y escalabilidad del sistema. |

Una vez definidas las Épicas que enmarcan la estrategia del producto, a continuación, se presenta la tabla detallada de Historias de Usuario:

### Tabla de Historias de Usuario

| ID | Título | Descripción | Criterios de Aceptación | ID Épica |
|----|--------|-------------|-----------------------------------------------|----------|
| US-001 | Registro con Email/SSO | Como nuevo usuario, quiero crear mi cuenta usando mi email o una red social **para acceder de manera rápida y segura a la plataforma**. | **Happy Path**: ***Given*** un usuario ingresa datos válidos en el formulario de registro, ***When*** confirma su registro, ***Then*** el sistema crea la cuenta y abre sesión automáticamente. <br> **Unhappy Path**: ***Given*** un usuario intenta registrarse con un email existente, ***When*** envía el formulario, ***Then*** el sistema muestra el mensaje de error “El email ya está en uso”. | EP01 |
| US-002 | Inicio de Sesión | Como usuario registrado, quiero iniciar sesión con mis credenciales **para acceder a mi panel personal sin inconvenientes**. | **Happy Path**: ***Given*** un usuario registrado ingresa su email y contraseña correctos, ***When*** selecciona “Iniciar Sesión”, ***Then*** el sistema lo redirige a su panel principal. <br> **Unhappy Path**: ***Given*** un usuario ingresa credenciales incorrectas, ***When*** intenta iniciar sesión, ***Then*** el sistema muestra el mensaje “Credenciales incorrectas” y no permite el acceso. | EP01 |
| US-003 | Recuperar Contraseña | Como usuario, quiero restablecer mi contraseña olvidada a través de mi email **para recuperar el acceso a mi cuenta de forma segura**. | **Happy Path**: ***Given*** un usuario ingresa un email registrado en la pantalla de recuperación, ***When*** solicita el restablecimiento, ***Then*** el sistema envía un email con un enlace para crear una nueva contraseña. <br> **Unhappy Path**: ***Given*** un usuario ingresa un email no registrado, ***When*** solicita el restablecimiento, ***Then*** el sistema muestra el mensaje “El email no se encuentra registrado”. | EP01 |
| US-004 | Completar Perfil de Dueño de vehículo | Como dueño de vehículo, quiero completar mi perfil con mi nombre y teléfono **para que los talleres puedan contactarme fácilmente**. | **Happy Path**: ***Given*** un dueño de vehículo autenticado abre su perfil, ***When*** guarda sus datos de contacto válidos, ***Then*** el sistema actualiza la información en su cuenta. | EP01 |
| US-005 | Alta de Vehículo | Como dueño de vehículo, quiero registrar mi vehículo (marca, modelo, año, placa) **para crear su garaje digital y organizar mejor mis mantenimientos**. | **Happy Path**: ***Given*** un dueño de vehículo en la sección “Mi Garaje”, ***When*** ingresa los datos válidos de un vehículo y guarda, ***Then*** el sistema agrega el vehículo a su lista. <br> **Unhappy Path**: ***Given*** un dueño de vehículo ingresa datos incompletos, ***When*** intenta guardar, ***Then*** el sistema muestra el mensaje “Complete todos los campos obligatorios”. | EP02 |
| US-006 | Registrar Lectura de Odómetro | Como dueño de vehículo, quiero registrar el kilometraje actual de mi vehículo **para alimentar el predictor y recibir recomendaciones de mantenimiento precisas**. | **Happy Path**: ***Given*** un dueño de vehículo selecciona un vehículo, ***When*** ingresa una lectura válida de odómetro y la guarda, ***Then*** el sistema añade la lectura al historial con fecha y hora. <br> **Unhappy Path**: ***Given*** un dueño de vehículo ingresa un valor no numérico, ***When*** intenta guardar, ***Then*** el sistema muestra el error “El valor de kilometraje no es válido”. | EP02 |
| US-007 | Cargar Historial Pasado | Como dueño de vehículo, quiero subir fotos de boletas antiguas y etiquetar servicios **para construir un historial inicial completo de mi vehículo**. | **Happy Path**: ***Given*** un dueño de vehículo sube la foto de una boleta, ***When*** etiqueta el servicio (ej. “Cambio de aceite”) con fecha y KM, ***Then*** el sistema crea un evento en el timeline del vehículo. | EP02 |
| US-008 | Ver Timeline de Servicios | Como dueño de vehículo, quiero ver el historial de mi vehículo en una línea de tiempo **para comprender fácilmente su historial de mantenimiento**. | **Happy Path**: ***Given*** un vehículo tiene servicios registrados, ***When*** el dueño de vehículo accede a su historial, ***Then*** el sistema muestra una lista cronológica de los eventos. | EP02 |
| US-009 | Filtrar Historial | Como dueño de vehículo, quiero filtrar el historial por tipo de servicio (ej. “frenos”) **para encontrar información específica rápidamente**. | **Happy Path**: ***Given*** un vehículo tiene múltiples servicios registrados, ***When*** el dueño de vehículo aplica el filtro “Frenos”, ***Then*** el sistema muestra únicamente esos servicios. | EP02 |
| US-010 | Descargar Comprobantes | Como dueño de vehículo, quiero descargar comprobantes (fotos, PDFs) de un servicio **para tener respaldo personal y administrativo**. | **Happy Path**: ***Given*** un servicio tiene un archivo adjunto, ***When*** el dueño de vehículo selecciona “Descargar”, ***Then*** el sistema descarga el archivo en su dispositivo. | EP02 |
| US-011 | Buscar Talleres | Como dueño de vehículo, quiero buscar talleres por cercanía o calificación **para encontrar la mejor opción de servicio para mi vehículo**. | **Happy Path**: ***Given*** un dueño de vehículo está en el mapa de talleres, ***When*** aplica el filtro “Más cercanos”, ***Then*** el sistema reordena la lista mostrando primero los más próximos. | EP03 |
| US-012 | Ver Perfil de Taller | Como dueño de vehículo, quiero ver el perfil de un taller (servicios, fotos, reseñas) **para decidir con confianza si agendar una cita**. | **Happy Path**: ***Given*** un dueño de vehículo selecciona un taller, ***When*** abre su perfil, ***Then*** el sistema muestra la información completa y comentarios de usuarios. | EP03 |
| US-013 | Reservar Cita | Como dueño de vehículo, quiero reservar un horario en un taller **para asegurar la atención de mi vehículo**. | **Happy Path**: ***Given*** un dueño de vehículo selecciona un horario disponible, ***When*** confirma la reserva, ***Then*** el sistema crea la cita, notifica al taller y envía confirmación al dueño de vehículo. <br> **Unhappy Path 1**: ***Given*** dos usuarios seleccionan el mismo horario, ***When*** ambos confirman, ***Then*** el sistema asigna el horario al primero y notifica al segundo “Horario no disponible”. <br> **Unhappy Path 2**: ***Given*** un usuario intenta reservar fuera del rango de atención, ***When*** confirma, ***Then*** el sistema muestra el error “Horario inválido”. | EP03 |
| US-014 | Reprogramar o Cancelar Cita | Como dueño de vehículo, quiero reprogramar o cancelar una cita con anticipación **para gestionar imprevistos sin penalidades**. | **Happy Path**: ***Given*** una cita es para dentro de 48 horas, ***When*** el dueño de vehículo solicita cancelación, ***Then*** el sistema la elimina sin penalidad. | EP03 |
| BS-001 | Configurar Perfil de Taller | Como jefe de taller, quiero configurar mi perfil público (dirección, horarios) **para atraer clientes y aumentar la visibilidad del taller**. | **Happy Path**: ***Given*** un jefe de taller autenticado, ***When*** actualiza descripción y fotos de su taller, ***Then*** el sistema refleja los cambios en el perfil público. | EP04 |
| BS-002 | Gestionar Agenda | Como jefe de taller, quiero ver mi agenda por día/semana **para planificar adecuadamente la recepción de vehículos**. | **Happy Path**: ***Given*** un taller tiene citas programadas, ***When*** el jefe de taller abre “Agenda Semanal”, ***Then*** el sistema muestra todas las citas distribuidas por día. | EP04 |
| BS-003 | Confirmar/Rechazar Cita | Como jefe de taller, quiero confirmar o rechazar nuevas solicitudes de cita **para mantener control sobre la carga de trabajo**. | **Happy Path**: ***Given*** el taller recibe una solicitud, ***When*** el jefe selecciona “Confirmar”, ***Then*** el sistema cambia el estado a “Confirmada” y notifica al cliente. | EP04 |
| BS-004 | Check-in de Vehículo | Como asesor de taller, quiero registrar el ingreso de un vehículo (KM, fotos) **para iniciar una OT y asegurar trazabilidad del servicio**. | **Happy Path**: ***Given*** un cliente llega con su vehículo, ***When*** el asesor realiza el check-in, ***Then*** el sistema crea una Orden de Trabajo en estado “En Proceso”. | EP04 |
| BS-005 | Registrar Ítems en OT | Como asesor de taller, quiero añadir ítems (mano de obra, repuestos) **para detallar el trabajo y garantizar transparencia en costos**. | **Happy Path**: ***Given*** una OT está “En Proceso”, ***When*** el asesor agrega un ítem válido, ***Then*** el sistema lo registra y recalcula el costo total. | EP04 |
| BS-006 | Adjuntar Evidencias a OT | Como asesor de taller, quiero adjuntar fotos del “antes” y “después” **para dar transparencia y fortalecer la confianza del cliente**. | **Happy Path**: ***Given*** una OT está abierta, ***When*** el asesor sube fotos, ***Then*** el sistema las guarda asociadas a la OT. | EP04 |
| BS-007 | Cerrar OT | Como asesor de taller, quiero cerrar una OT **para notificar al cliente y actualizar el historial del vehículo de manera correcta**. | **Happy Path**: ***Given*** una OT está completa, ***When*** el asesor la marca como “Finalizada”, ***Then*** el sistema actualiza el historial y notifica al cliente. <br> **Unhappy Path**: ***Given*** un asesor intenta cerrar una OT sin ítems registrados, ***When*** selecciona “Finalizar”, ***Then*** el sistema muestra el error “Debe registrar al menos un ítem antes de cerrar la OT”. | EP04 |
| BS-008 | Ver Calificaciones | Como jefe de taller, quiero ver calificaciones y comentarios **para medir el desempeño del taller y mejorar la atención al cliente**. | **Happy Path**: ***Given*** el taller tiene calificaciones registradas, ***When*** el jefe accede a “Reputación”, ***Then*** el sistema muestra el promedio y lista de comentarios. | EP04 |
| US-015 | Ver Próximo Servicio Sugerido | Como dueño de vehículo, quiero que el predictor me diga mi próximo mantenimiento **para planificar con anticipación y evitar averías**. | **Happy Path**: ***Given*** el vehículo tiene historial y KM actualizados, ***When*** el dueño de vehículo abre el panel principal, ***Then*** el sistema muestra una tarjeta con el próximo servicio sugerido. | EP05 |
| US-016 | Entender Recomendación | Como dueño de vehículo, quiero entender por qué se me recomienda un servicio **para confiar en la predicción y tomar decisiones informadas**. | **Happy Path**: ***Given*** el predictor sugiere un “Cambio de líquido de frenos”, ***When*** el dueño de vehículo selecciona “Ver por qué”, ***Then*** el sistema muestra la regla: “Recomendado cada 40,000 km”. | EP05 |
| US-017 | Ver Rango de Costo Estimado | Como dueño de vehículo, quiero ver un rango de costo estimado **para presupuestar y organizar mis gastos de mantenimiento**. | **Happy Path**: ***Given*** el predictor sugiere un servicio, ***When*** el dueño de vehículo abre los detalles, ***Then*** el sistema muestra un rango de precios (ej. S/ 380–460). | EP05 |
| BS-009 | Ver Checklist Sugerido | Como asesor de taller, quiero ver un checklist sugerido por el predictor **para preparar mejor la cita y garantizar un servicio completo**. | **Happy Path**: ***Given*** una cita vinculada a un servicio predicho, ***When*** el asesor abre sus detalles, ***Then*** el sistema muestra checklist recomendado. | EP05 |
| US-018 | Recibir Email de Confirmación | Como usuario, quiero recibir un email de confirmación al agendar una cita **para tener un respaldo claro de mi reserva**. | **Happy Path**: ***Given*** un usuario agenda cita exitosamente, ***When*** el sistema procesa la acción, ***Then*** envía un email con los detalles. | EP06 |
| US-019 | Recibir Notificación de Cierre | Como dueño de vehículo, quiero recibir una notificación in-app al finalizar el servicio **para estar informado en tiempo real del estado de mi vehículo**. | **Happy Path**: ***Given*** un taller cierra una OT, ***When*** el sistema registra la acción, ***Then*** envía una notificación al dueño de vehículo. | EP06 |
| AD-001 | Gestionar Tipos de Servicio | Como administrador, quiero crear o editar tipos de servicio **para mantener actualizado el catálogo maestro de la plataforma**. | **Happy Path**: ***Given*** un admin en “Catálogos”, ***When*** crea un nuevo servicio, ***Then*** el sistema lo deja disponible para talleres. | EP07 |
| AD-002 | Cargar Pautas de Mantenimiento | Como administrador, quiero cargar pautas por marca/modelo **para alimentar al predictor y mantener consistencia técnica**. | **Happy Path**: ***Given*** un admin tiene un CSV válido, ***When*** lo importa, ***Then*** el sistema incorpora las reglas al predictor. | EP07 |
| LP-001 | Entender la Propuesta de Valor | Como visitante, quiero entender en 30 segundos qué hace SmartCare **para decidir si registrarme**. | **Happy Path**: ***Given*** un visitante llega a la Landing Page, ***When*** lee el titular principal, ***Then*** comprende que la plataforma gestiona historial y predicciones. | EP08 |
| LP-002 | Ver Cómo Funciona | Como visitante, quiero ver pasos clave de uso **para evaluar si la plataforma es adecuada para mí**. | **Happy Path**: ***Given*** un visitante accede a “Cómo Funciona”, ***When*** la explora, ***Then*** el sistema muestra un resumen gráfico de los pasos. | EP08 |
| LP-003 | Ver Testimonios | Como visitante, quiero leer testimonios de otros usuarios **para generar confianza y seguridad en la plataforma**. | **Happy Path**: ***Given*** un visitante en la Landing Page, ***When*** accede a “Testimonios”, ***Then*** el sistema muestra citas y fotos de usuarios. | EP08 |
| LP-004 | Beneficios para Talleres | Como dueño de taller, quiero ver una sección con beneficios de afiliación **para decidir unirme a la red y atraer más clientes**. | **Happy Path**: ***Given*** un dueño de taller en la LP, ***When*** selecciona “Para Talleres”, ***Then*** el sistema lo dirige a la sección con beneficios. | EP08 |
| TS-001 | Configurar Entorno de Desarrollo | Como desarrollador, quiero un script de configuración local **para empezar a trabajar rápidamente en el proyecto**. | **Happy Path**: ***Given*** un desarrollador clona el repositorio, ***When*** ejecuta el script, ***Then*** el sistema instala dependencias y configura la BD local. | EP09 |
| TS-002 | Crear Schema de Base de Datos | Como desarrollador, quiero definir el esquema inicial de la BD **para persistir la información y soportar los módulos del sistema**. | **Happy Path**: ***Given*** migraciones definidas, ***When*** ejecuta el comando, ***Then*** el sistema crea tablas (Usuarios, Vehículos, Servicios). | EP09 |
| TS-003 | Implementar Endpoint de Autenticación | Como desarrollador, quiero implementar el endpoint de login con token JWT **para asegurar el acceso a las APIs**. | **Happy Path**: ***Given*** un usuario envía credenciales correctas a /api/auth/login, ***When*** el sistema procesa la solicitud, ***Then*** retorna un token JWT válido. <br> **Unhappy Path**: ***Given*** un usuario envía credenciales inválidas, ***When*** el sistema las procesa, ***Then*** retorna un código 401 “Unauthorized” con el mensaje “Credenciales incorrectas”. | EP09 |
| TS-004 | Implementar Lógica del Predictor | Como desarrollador, quiero implementar la primera versión del algoritmo predictivo basado en reglas **para generar recomendaciones iniciales de mantenimiento**. | **Happy Path**: ***Given*** un vehículo con 18,000 km y pauta cada 10,000 km, ***When*** el sistema ejecuta el predictor, ***Then*** sugiere “Cambio de aceite”. | EP09 |
| TS-005 | Desplegar API en Entorno de Pruebas | Como desarrollador, quiero desplegar la API en un servidor de pruebas **para que el equipo de frontend pueda integrarla**. | **Happy Path**: ***Given*** el código en la rama develop pasa pruebas y se ejecuta el pipeline, ***When*** el sistema despliega la API, ***Then*** la nueva versión queda disponible en la URL de pruebas. | EP09 |

## 3.3. Impact Mapping
En esta sección se presenta el Impact Mapping del modelo de negocio digital de SmartCare. Esta técnica de planificación estratégica es fundamental para alinear los objetivos de negocio con las funcionalidades a desarrollar, asegurando que cada característica del producto contribuya directamente a generar un cambio de comportamiento deseado en nuestros usuarios.

La estructura del mapa responde a las siguientes preguntas clave:
- **Goal (¿Por qué?)**: El objetivo de negocio medible que queremos alcanzar. 
- **Actor (¿Quién?)**: El User Persona que puede ayudarnos a lograr ese objetivo.
- **Impact (¿Cómo?)**: El cambio de comportamiento que esperamos ver en el actor.
- **Deliverable (¿Qué?)**: Las funcionalidades o características que construiremos para generar ese impacto.

A continuación, se presentan los mapas de impacto para cada uno de nuestros segmentos objetivo:

**Impact Map: Segmento Objetivo - Dueño de vehículo**

![Impact Mapping Conductor](../../assets/33-impact-mapping-conductor.jpg)

**Impract Map: Segmento Objetivo - Jefe/Asesor de Taller Afiliado**

![Impact Mapping Jefe Taller](../../assets/33-impact-mapping-jefe-taller.jpg)

## 3.4. Product Backlog

El Product Backlog organiza todas las historias priorizadas de acuerdo con el valor que generan para el negocio, siguiendo el enfoque incremental del desarrollo ágil. El orden refleja la estrategia de validar primero la propuesta de valor central (Historial + Predictor + Agenda), asegurar adopción inicial (Landing Page) y posteriormente incluir funcionalidades de soporte, reputación y técnicas.

| Orden | User Story Id | Título | Descripción | Story Points |
|-------|---------------|--------|-------------|--------------|
| 1 | US-005 | Alta de Vehículo | **Como** dueño de vehículo, **quiero** registrar mi vehículo **para** crear su garaje digital y organizar mantenimientos. | 3 |
| 2 | US-006 | Registrar Lectura de Odómetro | **Como** dueño de vehículo, **quiero** registrar el kilometraje actual **para** alimentar el predictor y recibir recomendaciones precisas. | 3 |
| 3 | US-015 | Ver Próximo Servicio Sugerido | **Como** dueño de vehículo, **quiero** que el predictor me indique mi próximo mantenimiento **para** planificar con anticipación. | 5 |
| 4 | US-016 | Entender Recomendación | **Como** dueño de vehículo, **quiero** entender por qué se recomienda un servicio **para** confiar en el predictor. | 2 |
| 5 | US-017 | Ver Rango de Costo Estimado | **Como** dueño de vehículo, **quiero** ver un rango de costo estimado **para** presupuestar mis mantenimientos. | 3 |
| 6 | US-007 | Cargar Historial Pasado | **Como** dueño de vehículo, **quiero** subir boletas antiguas **para** construir el historial inicial de mi vehículo. | 5 |
| 7 | US-008 | Ver Timeline de Servicios | **Como** dueño de vehículo, **quiero** visualizar el historial de servicios en una línea de tiempo **para** comprender su mantenimiento. | 3 |
| 8 | US-009 | Filtrar Historial | **Como** dueño de vehículo, **quiero** filtrar el historial por tipo de servicio **para** encontrar información específica. | 2 |
| 9 | US-010 | Descargar Comprobantes | **Como** dueño de vehículo, **quiero** descargar comprobantes asociados **para** tener un respaldo. | 2 |
| 10 | US-011 | Buscar Talleres | **Como** dueño de vehículo, **quiero** buscar talleres por cercanía o calificación **para** elegir la mejor opción. | 3 |
| 11 | US-012 | Ver Perfil de Taller | **Como** dueño de vehículo, **quiero** ver el perfil de un taller con reseñas **para** decidir si agendar. | 2 |
| 12 | US-013 | Reservar Cita | **Como** dueño de vehículo, **quiero** reservar un horario en un taller **para** asegurar la atención. | 5 |
| 13 | US-014 | Reprogramar o Cancelar Cita | **Como** dueño de vehículo, **quiero** reprogramar o cancelar citas **para** gestionar imprevistos. | 3 |
| 14 | US-018 | Recibir Email de Confirmación | **Como** usuario, **quiero** recibir confirmación por email al agendar una cita **para** tener un respaldo. | 2 |
| 15 | US-019 | Recibir Notificación de Cierre | **Como** dueño de vehículo, **quiero** recibir notificación al finalizar un servicio **para** estar informado. | 2 |
| 16 | LP-001 | Entender la Propuesta de Valor | **Como** visitante, **quiero** entender en 30 segundos qué hace SmartCare **para** decidir si registrarme. | 2 |
| 17 | LP-002 | Ver Cómo Funciona | **Como** visitante, **quiero** ver pasos clave de uso **para** evaluar si la plataforma es para mí. | 2 |
| 18 | LP-003 | Ver Testimonios | **Como** visitante, **quiero** leer testimonios de otros usuarios **para** confiar en la plataforma. | 1 |
| 19 | LP-004 | Beneficios para Talleres | **Como** dueño de taller, **quiero** conocer beneficios de afiliarme **para** decidir unirme. | 2 |
| 20 | BS-001 | Configurar Perfil de Taller | **Como** jefe de taller, **quiero** configurar el perfil público **para** atraer clientes. | 3 |
| 21 | BS-002 | Gestionar Agenda | **Como** jefe de taller, **quiero** ver mi agenda por día/semana **para** planificar la recepción de vehículos. | 3 |
| 22 | BS-003 | Confirmar/Rechazar Cita | **Como** jefe de taller, **quiero** confirmar o rechazar solicitudes de cita **para** mantener control. | 2 |
| 23 | BS-004 | Check-in de Vehículo | **Como** asesor de taller, **quiero** registrar el ingreso de un vehículo **para** iniciar una OT. | 3 |
| 24 | BS-005 | Registrar Ítems en OT | **Como** asesor de taller, **quiero** añadir ítems a una OT **para** detallar el trabajo. | 3 |
| 25 | BS-006 | Adjuntar Evidencias a OT | **Como** asesor de taller, **quiero** adjuntar fotos en una OT **para** dar transparencia. | 2 |
| 26 | BS-007 | Cerrar OT | **Como** asesor de taller, **quiero** cerrar una OT **para** notificar al cliente y actualizar historial. | 3 |
| 27 | BS-008 | Ver Calificaciones | **Como** jefe de taller, **quiero** ver calificaciones y comentarios **para** mejorar la atención. | 2 |
| 28 | BS-009 | Ver Checklist Sugerido | **Como** asesor de taller, **quiero** ver checklist sugerido por el predictor **para** preparar mejor una cita. | 3 |
| 29 | AD-001 | Gestionar Tipos de Servicio | **Como** administrador, **quiero** crear/editar tipos de servicio **para** mantener catálogo actualizado. | 2 |
| 30 | AD-002 | Cargar Pautas de Mantenimiento | **Como** administrador, **quiero** cargar pautas por marca/modelo **para** alimentar al predictor. | 3 |
| 31 | TS-001 | Configurar Entorno de Desarrollo | **Como** desarrollador, **quiero** un script de configuración local **para** iniciar rápido. | 2 |
| 32 | TS-002 | Crear Schema de Base de Datos | **Como** desarrollador, **quiero** definir el esquema inicial de BD **para** persistir información. | 3 |
| 33 | TS-003 | Implementar Endpoint de Autenticación | **Como** desarrollador, **quiero** un endpoint de login con token JWT **para** asegurar las APIs. | 5 |
| 34 | TS-004 | Implementar Lógica del Predictor | **Como** desarrollador, **quiero** implementar algoritmo predictivo inicial **para** generar recomendaciones. | 5 |
| 35 | TS-005 | Desplegar API en Entorno de Pruebas | **Como** desarrollador, **quiero** desplegar la API en un servidor de pruebas **para** integración de frontend. | 3 |
