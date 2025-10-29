# Indice

- [Gestión de la iteración](#gestión-de-la-iteración)
  - [Definición del marco de trabajo](#definición-del-marco-de-trabajo)
  - [Planificación de la iteración](#planificación-de-la-iteración)
  - [Seguimiento de la iteración](#seguimiento-de-la-iteración)
  - [Inspección y adaptación del proceso](#inspección-y-adaptación-del-proceso)
- [Construir y validar posibles soluciones del MVP a través de prototipos](#construir-y-validar-posibles-soluciones-del-mvp-a-través-de-prototipos)
  - [Prototipos con posibles soluciones](#prototipos-con-posibles-soluciones)
  - [Inspección y adaptación del producto](#inspección-y-adaptación-del-producto)

# Gestión de la iteración

## Definición del marco de trabajo

Siguiendo como habíamos establecido los roles con la intención de que en las siguientes iteraciones se roten, favoreciendo así la participación y el aprendizaje de todos.

- **Product Owner**: Juan Croquis

- **Scrum Master**: Juan Ferreira

- **Developer**:  Emiliano Reyes

### Artefactos principales

En el presente Sprint definimos que los eventos se establecerán de la siguiente forma:

- **Sprint Planning**: 2 días (27/10/2025 y )
- **Daily Scrum**: 3 días ()
- **Sprint Review**: 1 día ()
- **Sprint Retrospective**: 1 día ()

# Definition of Done y Definition of Ready – Carpool Universitario

## Definition of Done (DoD)

Un entregable (historia de usuario, funcionalidad o tarea) se considera **terminado** cuando:

- **Funcionalidad implementada**  
  Ejemplo: el registro de usuario permite crear cuenta como conductor o pasajero.  

- **Funcionalidad testeada**  
  Pruebas unitarias y funcionales confirman que el login, búsqueda de viajes, reserva y publicación funcionan según lo esperado.  

- **Criterios de aceptación cumplidos**  
  Cada historia de usuario cuenta con criterios claros (ejemplo:  
  *“Como pasajero quiero buscar un viaje por horario y zona, para elegir la mejor opción”*),  
  y deben cumplirse en su totalidad.  

---

## Definition of Ready (DoR)

Una historia de usuario o tarea se considera **lista para entrar en un Sprint** cuando:

- **Estimación de esfuerzo confirmada**  
  El equipo acordó una estimación en puntos de historia o tiempo, y está alineada con la capacidad disponible del Sprint.  

- **Recursos disponibles**  
  El equipo cuenta con acceso a las herramientas necesarias.

- **Conocimientos/capacitación suficiente**  
  Los miembros tienen claro cómo implementar la historia.

- **Diseño de UI aprobado**  
  Las pantallas necesarias para la historia (ejemplo: formulario de *Publicar viaje*, vista de *Reservar lugar*) están definidas y detalladas.  

- **Criterios de aceptación definidos**  
  Cada historia de usuario tiene escenarios claros que permitan saber cuándo está “hecha”. 

## Planificación de la iteración

### Minuta 1: Planning 1 (27/10/2025)

Lunes 27 de Octubre, realizamos la primera reunión para preparar el ambiente para la iteración 3. El objetivo de esta reunión fue avanzar y planificar qué íbamos a realizar en esta iteración (Sprint). Designamos roles, validamos las herramientas a utilizar, definimos el objetivo de la iteración, buscamos consenso sobre cómo aplicar el marco de trabajo SCRUM al contexto del proyecto y qué corresponde a cada rol y dejamos preparado el **Product Backlog**. La reunión se dio en clases, duró 30 minutos y concluimos que en la siguiente reunión continuaremos con la siguiente parte del planning.

![Planning 1](Reuniones/Planing1.PNG "Planning 1")


### Sprint Backlog

![B1](Backlog/B1.PNG "B1")
![B2](Backlog/B2.PNG "B2")
![B3](Backlog/B3.PNG "B3")
![B4](Backlog/B4.PNG "B4")

#### 👥 Asignación de tareas

Durante la **planificación** asumimos distintos roles según la necesidad, pero en la etapa de **desarrollo** trabajaremos los tres de forma colaborativa.  
Repartimos las tareas de manera **equitativa**, asegurando que cada integrante comience con una **tarea de prioridad 1**.

#### 📚 Historias de usuario

- **Historia de usuario 12**: Login con cuenta de Google
  - **Como**: Como usuario registrado (conductor o pasajero)
  - **Quiero**: Iniciar sesión con mi usuario de Google para acceder a mis viajes y reservas.
  - **Para**: Poder acceder a mis viajes publicados, reservas o búsqueda de viajes y perfil personal.
  - **Criterios de aceptación**:
    - El botón de Continuar con Google debe redirigir a un panel a parte.
    - Al iniciar sesión correctamente, se redirige al usuario a su pantalla principal donde seleccionará su perfil (conductor o pasajero).

- **Historia de usuario 17**: Evaluar pasajeros según criterios
  - **Como**: Conductor que ha finalizado un viaje
  - **Quiero**: Seleccionar a cada pasajero y calificar su comportamiento o cumplimiento durante el viaje
  - **Para**: Mantener un registro de buenas prácticas, mejorar la confianza y seguridad dentro de la comunidad de usuarios
  - **Criterios de aceptación**:
    - Al finalizar un viaje, el conductor puede acceder a la pantalla de historial y ver la lista de pasajeros.
    - Debe poder seleccionar un pasajero específico y asignarle una calificación en estrellas (1 a 5).
    - Opcionalmente puede escribir una breve reseña o comentario.
    - El sistema debe permitir iniciar una disputa si el conductor tuvo un problema con un pasajero.

- **Historia de usuario 21**: Evaluar al conductor luego del viaje
  - **Como**: Pasajero que ha finalizado un viaje
  - **Quiero**: Calificar la experiencia con mi conductor y dejar una reseña breve
  - **Para**: Contribuir a la reputación del conductor y mejorar la calidad del servicio para futuros usuarios
  - **Criterios de aceptación**:
    - Al finalizar un viaje, debe mostrarse la pantalla de historial con los datos del conductor y la opción de "Enviar reseña".
    - El pasajero puede asignar una calificación en estrellas (1 a 5).
    - Opcionalmente puede escribir una breve reseña o comentario.
    - El pasajero tendrá la opción de abrir un debate si hubo un problema.

> **Nota:** Se añadieron las tasks de redacción de historias de usuarios correspondientes a las cards que vamos a trabajar durante esta Iteración 3, además de la creación de pantallas intermedias necesarias para conectar las pantallas creadas.

Para estimar el esfuerzo de las historias seleccionadas aplicamos la técnica **Planning Poker** basada en **Story Points**.

Tomamos en cuenta los siguientes factores:
- **Complejidad técnica**
- **Volumen de trabajo**
- **Nivel de incertidumbre**

Utilizamos el **estimador integrado en Azure DevOps** para asignar valores dentro de cada historia elegida para el sprint.  
En los casos donde hubo diferencias de criterio, el equipo **debatió las estimaciones** y se realizó **una nueva votación** hasta llegar a un consenso.

A continuación se redactan las estimaciones puestas por el equipo correspondientes a estas Historias de Usuarios (Como definimos antes 1 SP corresponde a 30 minutos).

- **Historia de usuario 12**: Login con cuenta de Google
  - 5 SP
- **Historia de usuario 13**: Editar usuario
  - 5 SP
- **Historia de usuario 15**: Recuperar contraseña
  - 7 SP
- **Historia de usuario 17**: Evaluar pasajeros según criterios
  - 3 SP
- **Historia de usuario 19**: Cancelar viaje/s publicados
  - 4 SP
- **Historia de usuario 21**: Evaluar al conductor luego del viaje
  - 3 SP
- **Historia de usuario 24**: Gestionar reportes de la comunidad
  - 6 SP
- **Historia de usuario 25**: Resolver discrepancias en evaluaciones
  - 6 SP
- **Historia de usuario 28**: Recordatorio a pasajeros con reserva
  - 5 SP
- **Historia de usuario 33**: Historial de viajes realizados
(Conductor)
  - 4 SP
- **Historia de usuario 36**: Cancelar reserva
  - 5 SP
- **Historia de usuario 37**: Historial de viajes realizados
(Pasajero)
  - 4 SP

### Artefactos principales

- Minuta de la sprint planning con su agenda, actividades y resultados.
- Objetivos de la iteración.
- Sprint backlog con historias de usuarios y tareas asociadas.
- Planificación de acuerdo a la capacidad del equipo.
- Técnicas de priorización y estimación utilizadas.
- Uso de métricas relevantes para la planificación como la velocidad y productividad.

## Seguimiento de la iteración

_[Existe evidencia sobre el registro de actividades y horas de cada integrante del equipo con el seguimiento general de cada iteración del proyecto sobre lo planificado inicialmente.]_

### Artefactos principales

- Minuta de daily scrum describiendo la coordinación del trabajo de cada integrante del equipo.
  - ¿Que logramos hacer?
  - ¿Qué planificamos hacer?
  - ¿Qué impedimentos tenemos?
- Registro y reporte de horas de cada integrante del equipo con sus actividades principales.
- Seguimiento visual de la iteración con burndown y/o burnup charts.

## Inspección y adaptación del proceso

_[Existe evidencia sobre la inspección del proceso con aprendizajes principales y acciones de mejora implementadas durante el desarrollo del proyecto.]_

### Artefactos principales

- Minuta de la retrospectiva con la dinámica utilizada y sus principales resultados.
- Planificación y seguimiento de las acciones de mejora.

# Construir y validar posibles soluciones del MVP a través de prototipos

## Prototipos con posibles soluciones

_[Existen diferentes propuestas de solución para entregar valor y resolver el problema identificado implementado a través de prototipos. Los prototipos deberán ser exportados en algún formato de imagen (como png o jpg) a efectos de poder ser visualizados fácilmente dentro del propio repo de github.]_

### Artefactos principales

- Prototipos interactivos para ser navegados.
- Prototipos asociados como bocetos a las historias de usuario.

## Inspección y adaptación del producto

_[Existe evidencia de instancias de inspección y validación del producto con usuarios y la recolección de su feedback con ajustes finales a los prototipos.]_

### Artefactos principales

- Minutas de sprint review.
- Evidencia de los usability testing con usuarios finales.
  - Descripción de las tareas propuestas a los usuarios finales.
  - Cobertura obtenida de validación de los usuarios de la aplicación.
- Feedback recibido de los usuarios finales con la priorización de las propuestas de cambio.
