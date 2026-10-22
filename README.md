# 🚕 Al Toque — Aplicación móvil de solicitudes de taxi

**Proyecto académico de Ingeniería Informática | Flutter · Dart · Firebase · Google Maps**

Al Toque es un prototipo de aplicación móvil orientado a la gestión de solicitudes de servicios de taxi, desarrollado en el contexto de un proyecto de tesis de Ingeniería Informática.

El proyecto busca facilitar la interacción entre pasajeros y conductores mediante una aplicación que permite solicitar viajes, recibir solicitudes, consultar recorridos y administrar información relacionada con los servicios de transporte.

> **Estado del proyecto:** prototipo académico. La aplicación no se encuentra actualmente desplegada como un servicio comercial.

## 📌 Contexto del proyecto

El proyecto se desarrolló tomando como referencia las necesidades de la **Asociación de Transporte Libre Radio Móvil San Pedro Ltda.**, ubicada en Yacuiba, Bolivia.

La propuesta contempla dos perfiles principales:

- **Pasajero:** permite solicitar un servicio de taxi, visualizar información del viaje y consultar su estado.
- **Conductor:** permite recibir solicitudes, visualizar recorridos y gestionar el desarrollo del servicio.

El objetivo académico fue estudiar y aplicar tecnologías de desarrollo móvil y servicios en la nube a un caso práctico de transporte local.

## 🛠️ Tecnologías utilizadas

| Tecnología | Aplicación en el proyecto |
|---|---|
| Flutter | Desarrollo de la aplicación móvil |
| Dart | Programación y lógica de la aplicación |
| Firebase Authentication | Autenticación de usuarios |
| Cloud Firestore | Almacenamiento y consulta de información |
| Firebase Cloud Messaging | Integración de notificaciones |
| Firebase Storage | Gestión de archivos |
| Google Maps | Visualización de mapas y recorridos |
| Geolocator y Geocoding | Geolocalización y tratamiento de ubicaciones |
| Lottie | Animaciones de interfaz |

## 📱 Funcionalidades del prototipo

### Módulo de pasajeros

- Registro e inicio de sesión.
- Visualización de mapas.
- Selección de ubicaciones y solicitud de taxi.
- Búsqueda y asignación de conductor.
- Visualización del estado de una solicitud.
- Seguimiento del recorrido.
- Finalización y calificación del servicio.
- Gestión de información del perfil.

### Módulo de conductores

- Registro e inicio de sesión.
- Visualización del mapa y ubicación.
- Recepción de solicitudes de servicio.
- Consulta de información del pasajero.
- Visualización de rutas.
- Inicio y finalización de viajes.
- Calificación del pasajero.
- Consulta de información de viajes.

**Nota:** estas funcionalidades corresponden a módulos representados en el prototipo. No se afirma que todos los flujos estén actualmente operativos o probados de extremo a extremo.

## 📸 Capturas de pantalla

Las siguientes imágenes muestran diferentes interfaces del prototipo.

### 1. Experiencia del pasajero

**Solicitud y asignación de taxi**

<p>
  <img src="docs/capturas/solicitud-taxi-mapa.png" width="220" alt="Mapa para solicitar taxi">
  <img src="docs/capturas/confirmacion-solicitud-y-ruta.png" width="220" alt="Confirmación de solicitud y recorrido">
  <img src="docs/capturas/buscando-conductor.png" width="220" alt="Búsqueda de conductor">
  <img src="docs/capturas/conductor-acepta-ruta.png" width="220" alt="Aceptación de solicitud">
</p>

**Seguimiento y finalización del servicio**

<p>
  <img src="docs/capturas/viaje-en-curso-pasajero.png" width="220" alt="Viaje en curso">
  <img src="docs/capturas/viaje-finalizado-calificar-conductor.png" width="220" alt="Calificación del conductor">
  <img src="docs/capturas/editar-perfil-pasajero.png" width="220" alt="Edición del perfil">
</p>

### 2. Experiencia del conductor

**Disponibilidad y recepción de solicitudes**

<p>
  <img src="docs/capturas/mapa-conductor-disponible.png" width="220" alt="Mapa del conductor">
  <img src="docs/capturas/solicitud-recibida-conductor.png" width="220" alt="Solicitud recibida">
</p>

**Gestión del recorrido**

<p>
  <img src="docs/capturas/ruta-conductor-iniciar-viaje.png" width="220" alt="Ruta para iniciar el viaje">
  <img src="docs/capturas/ruta-conductor-finalizar-viaje.png" width="220" alt="Ruta para finalizar el viaje">
  <img src="docs/capturas/detalle-cliente-y-recorrido.png" width="220" alt="Detalle del cliente y recorrido">
  <img src="docs/capturas/detalle-conductor-y-recorrido.png" width="220" alt="Detalle del conductor y recorrido">
  <img src="docs/capturas/viaje-finalizado-calificar-cliente.png" width="220" alt="Calificación del cliente">
</p>

> Las capturas se presentan con fines de documentación académica. Algunas pantallas contienen mapas, ubicaciones o recorridos, por lo que fueron censuradas antes de su publicación para evitar revelar información sensible.

## 🏗️ Arquitectura general

La aplicación utiliza una estructura basada en componentes y clases que organizan las responsabilidades principales:

- **Pantallas (Pages):** interfaces correspondientes a las funcionalidades del pasajero y del conductor.
- **Controladores (Controllers):** gestión de eventos, navegación y lógica asociada a las pantallas.
- **Modelos (Models):** representación de las entidades y estructuras de datos.
- **Proveedores (Providers):** comunicación con los servicios externos y acceso a la información.
- **Servicios Firebase:** autenticación, persistencia de datos y mensajería.

Esta organización permite separar parcialmente la presentación, la lógica de aplicación y el acceso a servicios externos.

## 💻 Contribuciones técnicas y adaptaciones

Al Toque se desarrolló tomando como punto de partida una aplicación de ejemplo de un curso de Flutter disponible en Udemy. Este material proporcionó una base funcional que posteriormente fue adaptada al contexto del proyecto académico.

Durante el desarrollo se identificaron las siguientes contribuciones y modificaciones:

### 1. Historial de viajes del conductor

Se incorporaron pantallas y controladores destinados a consultar el historial de viajes realizados por un conductor.

Esta adaptación incluyó:

- Implementación de interfaces para visualizar viajes registrados.
- Incorporación de una pantalla de detalle del viaje.
- Reutilización de modelos y proveedores de datos existentes.
- Integración de las nuevas pantallas con la estructura de navegación de la aplicación.

### 2. Adaptación de la interfaz de usuario

Se realizaron modificaciones visuales para adecuar la aplicación al contexto del servicio de transporte local.

Entre ellas:

- Personalización de la identidad visual.
- Modificación de textos y elementos de presentación.
- Adaptación de la pantalla de entrada y selección de perfiles.
- Incorporación de una animación de presentación utilizando Lottie.

### 3. Mantenimiento y adaptación del código

Durante el trabajo con el proyecto base se realizaron ajustes relacionados con:

- Manejo de tipos anulables (*null safety*) en Dart.
- Modificaciones en controladores y navegación.
- Adaptaciones necesarias para trabajar con el código y las dependencias del proyecto.

### 4. Integración y comprensión de servicios

El proyecto permitió trabajar con la estructura de una aplicación Flutter que utiliza Firebase y Google Maps, incluyendo:

- Autenticación de usuarios.
- Almacenamiento y consulta de datos.
- Representación de ubicaciones y recorridos.
- Comunicación con servicios externos.

Estas integraciones forman parte de la aplicación base y del trabajo de adaptación académica; no se presentan como implementaciones desarrolladas íntegramente desde cero.

### Alcance de las contribuciones

Las modificaciones descritas corresponden a diferencias identificadas respecto al material original del curso. El proyecto se presenta como una experiencia de aprendizaje, integración y adaptación de software en un contexto académico.

## 🎯 Conocimientos aplicados

El desarrollo de Al Toque permitió trabajar con conceptos y tecnologías relacionados con:

- Desarrollo de aplicaciones móviles multiplataforma.
- Integración de servicios en la nube.
- Autenticación y administración de usuarios.
- Persistencia de información en bases de datos NoSQL.
- Consumo e integración de servicios externos.
- Geolocalización y representación de recorridos.
- Organización de código mediante modelos, controladores y proveedores.
- Diseño y adaptación de interfaces móviles.

## 📋 Alcance del repositorio

Este repositorio está destinado a la **presentación técnica y visual del proyecto académico**.

No contiene el código fuente completo de la aplicación ni archivos de configuración con credenciales.

La redistribución del código utilizado como base de aprendizaje está sujeta a la licencia o autorización correspondiente.

## 👨‍💻 Autor

**Juan Bautista Padilla Caihuara**

Ingeniería Informática  
Universidad Autónoma Juan Misael Saracho  
Yacuiba, Bolivia

**Enlaces:**

- [GitHub](https://github.com/juanbpadilla)
- [LinkedIn](https://www.linkedin.com/in/juan-padilla-ba013a17a/)

---

*Al Toque — Proyecto académico de Ingeniería Informática.*
