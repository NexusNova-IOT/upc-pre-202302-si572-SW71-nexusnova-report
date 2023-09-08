<div align="justify">
## 4.1. Strategic-Level Domain-Driven Design

En el siguiente apartado, se detalla una serie de enfoques clave en el proceso de Diseño Dirigido por el Dominio a nivel estratégico (Strategic-Level Domain-Driven Design). Estos enfoques desempeñaron un papel fundamental en el establecimiento de una base sólida para la definición y modelado de dominios complejos. A través de técnicas como Event Storming, Context Mapping y la definición de la Arquitectura de Software, se logró obtener una comprensión profunda de los elementos esenciales necesarios para la creación de sistemas efectivos y bien estructurados. A continuación, se describen los puntos clave que se abordaron en esta sección.

### 4.1.1. EventStorming

Se abordó un enfoque colaborativo y visual que permitió modelar el contexto del dominio. Se exploraron las etapas de Candidate Context Discovery, Domain Message Flows Modeling y la creación de Bounded Context Canvases.

#### Unstructured Exploration
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/unstructured-exploration.png" width ="700px" alt="unstructured-exploration-step" style="margin-right: 20px;">
</div>

#### Pain points
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/pain-points.png" width ="700px" alt="pain-points-step" style="margin-right: 20px;">
</div>

#### Timelines
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/timelines.png" width ="700px" alt="timelines-step" style="margin-right: 20px;">
</div>

#### Pivotal points
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/pivotal-point.png" width ="700px" alt="pivotal-points-step" style="margin-right: 20px;">
</div>

#### Commands
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/commands.png" width ="700px" alt="commands-step" style="margin-right: 20px;">
</div>

#### Policies
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/policies.png" width ="700px" alt="policies-step" style="margin-right: 20px;">
</div>

#### Read Models
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/read-models.png" width ="700px" alt="read-models-step" style="margin-right: 20px;">
</div>

#### External Systems
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/external-systems.png" width ="700px" alt="external-systems-step" style="margin-right: 20px;">
</div>

#### Aggregates
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/event-storming/raggregates.png" width ="700px" alt="aggregates-step" style="margin-right: 20px;">
</div>


#### 4.1.1.1 Candidate Context Discovery.
Empleando la metodología de eventstorming con enfoque en la técnica de "start-with-simple", utilizamos la línea de tiempo para identificar posibles candidatos para nuestro contexto delimitado, los cuales son Perfil, Creación y edición de diseños y Gestión de diseños.

#### 4.1.1.2 Domain Message Flows Modeling.
Durante este procedimiento, se detectaron los participantes, mensajes que secomparten y se delinean en las corrientes de información que enlazan estos componentes.

##### 1. Scenario: Registering in the app
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-1.png" width ="700px" alt="flow-1" style="margin-right: 20px;">
</div>

##### 2. Scenario: Registering in the app
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-2.png" width ="700px" alt="flow-2" style="margin-right: 20px;">
</div>

##### 3. Scenario: Pay a Tour Package
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-3.png" width ="700px" alt="flow-3" style="margin-right: 20px;">
</div>

##### 4. Scenario: Pay a Subscription
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-4.png" width ="700px" alt="flow-4" style="margin-right: 20px;">
</div>

##### 5. Scenario: Register a Ground Transportation Vehicle
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-5.png" width ="700px" alt="flow-5" style="margin-right: 20px;">
</div>

##### 6. Scenario: Assign a vehicle for a Tour Package
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-6.png" width ="700px" alt="flow-6" style="margin-right: 20px;">
</div>

##### 7. Scenario: Reassign a vehicle for excess weight limit
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-7.png" width ="700px" alt="flow-7" style="margin-right: 20px;">
</div>

##### 8. Scenario: Locate a Tourist
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-9.png" width ="700px" alt="flow-9" style="margin-right: 20px;">
</div>

##### 9. Scenario: Alert the tourist about the weather of the place of the tour
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-10.png" width ="700px" alt="flow-10" style="margin-right: 20px;">
</div>

##### 10. Scenario: Check purchased tour packages
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/domain-message-flows-modeling/flow-11.png" width ="700px" alt="flow-11" style="margin-right: 20px;">
</div>

#### 4.1.1.3 Bounded Context Canvases.

### 4.1.2. Context Mapping

Después de obtener cuáles serían nuestros Bounded Contexts, se realizó la elaboración de las relaciones estructurales entre estos. Para ello, se tomó en cuenta posibles diseños candidatos para el Context Mapping, el cual se desarrolló considerando los patrones de relaciones entre Bounden Contexts establecidos en Domain-Driven Desgin, como Conformist, Customer/Supplier, Partnership o Shared Kernel. Se utilizó la herramienta online DomoRoboto para elaborar el Context Mapping de la siguiente imagen: 

<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/context-mapping/context-mapping.png" width ="700px" alt="context-mapping" style="margin-right: 20px;">
</div>

### 4.1.3. Software Architecture

Se presentaron diversas perspectivas arquitectónicas que ayudaron a visualizar y estructurar sistemas de software. Se exploraron diagramas a nivel de Paisaje del Sistema, Nivel de Contexto y Nivel de Contenedor, así como Diagramas de Despliegue que arrojaron luz sobre la infraestructura en la que operaría el sistema.

#### 4.1.3.1. Software Architecture System Landscape Diagram.
Se realizó un System Landscape Diagram con el objetivo de visualizar una relación general entre el sistema interno, externos y los usuarios.
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/c4-model/landscape.png" width ="700px" alt="landscape-diagram" style="margin-right: 20px;">
</div>

#### 4.1.3.2. Software Architecture Context Level Diagrams.
Se realizó el primer nivel de Software Architecture, System Context en la herramienta Structuriz como se muestra en la siguiente imagen. 
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/c4-model/context.png" width ="700px" alt="context-diagram" style="margin-right: 20px;">
</div>

#### 4.1.3.2. Software Architecture Container Level Diagrams.
Se realizó el segundo nivel de Software Architecture, Container, en la herramienta Structuriz como se muestra en la siguiente imagen. 
<div style="display: flex; align-items: center;">
    <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/c4-model/container.png" width ="700px" alt="context-mapping" style="margin-right: 20px;">
</div>

#### 4.1.3.3. Software Architecture Deployment Diagrams.


## 4.2. Tactical-Level Domain-Driven Design
### 4.2.1. Bounded Context: Profile management
Este bounded context se centra en las clases y capas relacionadas con la gestión de perfiles de usuario, permitiendo a los usuarios ver y actualizar su información de perfil. A continuación, se detallan las principales componentes de este contexto:
#### 4.2.1.1. Domain Layer.
- **UserProfile:** Esta clase representa el perfil del usuario y contiene atributos como nombre, apellidos, dirección de correo electrónico, número de teléfono, foto de perfil, y otros detalles personales. También puede incluir métodos para actualizar la información del perfil.
- **ProfilePrivacySettings:** Esta clase define la configuración de privacidad del perfil, que permite a los usuarios controlar quién puede ver ciertos elementos de su perfil.
- **ProfileActivity:** Esta clase registra la actividad del usuario en su perfil, como cambios de foto de perfil, actualizaciones de información, etc. Esto puede ayudar a rastrear el historial de actividad del perfil.


*Enum:*
- **PrivacyLevel:** Este enum define los niveles de privacidad posibles para elementos del perfil, como público, privado, solo amigos, etc.
#### 4.2.1.2. Interface Layer.
- **ProfileViewController:** Este controlador maneja las solicitudes relacionadas con la visualización del perfil del usuario. Permite a los usuarios ver su información de perfil y configurar la privacidad de sus datos.
- **ProfileUpdateController:** Este controlador se encarga de las solicitudes de actualización de información de perfil. Facilita a los usuarios la capacidad de modificar su información personal, incluyendo la foto de perfil.




#### 4.2.1.3. Application Layer.
- **ProfileViewService:** Este servicio de aplicación se encarga de procesar las solicitudes de visualización de perfiles de usuario. Accede a la base de datos para recuperar la información del perfil y aplica las configuraciones de privacidad antes de mostrarla al usuario.
- **ProfileUpdateService:** Se encarga de procesar las solicitudes de actualización de información de perfil. Valida los cambios propuestos por el usuario, actualiza los datos en la base de datos y registra la actividad correspondiente en el perfil.


#### 4.2.1.4. Infrastructure Layer.
- **ProfileRepository:** Su principal función es interactuar con la base de datos para realizar operaciones de lectura y escritura de información de perfiles de usuario. Almacena y recupera datos de perfil, configuraciones de privacidad y actividad.
- **ImageStorageService:** Este servicio se encarga de almacenar y recuperar imágenes de perfil de usuario, como las fotos de perfil. Puede estar conectado a un sistema de almacenamiento de objetos para gestionar eficazmente las imágenes.
- **PrivacySettingsRepository:** Almacena y recupera la configuración de privacidad de los perfiles de usuario.
- **ActivityLogRepository:** Registra y recupera la actividad del perfil de usuario.
#### 4.2.1.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
   <img src="https://raw.githubusercontent.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/tb1/Resources/diagrams/Profile%20BC%20Component%20Diagram.png"       width ="700px" alt="Imagen" style="margin-right: 20px;">
</div>

#### 4.2.1.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.1.6.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.1.6.2. Bounded Context Database Design Diagram.


### 4.2.2. Bounded Context: Tour Experience
En esta sección, presentaremos la propuesta táctica para el diseño de la solución de software en el contexto de "Profile Management". Detallaremos las clases identificadas y explicaremos sus atributos, métodos y relaciones, siguiendo una estructura que abarca las diferentes capas de nuestra arquitectura.

#### 4.2.2.1. Domain Layer.
#### 4.2.2.2. Interface Layer.
#### 4.2.2.3. Application Layer.
#### 4.2.2.4. Infrastructure Layer.
#### 4.2.2.5. Bounded Context Software Architecture Component Level Diagrams.

<div style="display: flex; align-items: center;">
    <img src="./resources/images/diagrams/../../diagrams/Tour%20Experience%20BC%20Component%20Diagram.png"     width ="700px" alt="Imagen" style="margin-right: 20px;">

    
</div>

#### 4.2.2.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.2.6.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.2.6.2. Bounded Context Database Design Diagram.


### 4.2.3. Bounded Context: Transportation
#### 4.2.3.1. Domain Layer.
#### 4.2.3.2. Interface Layer.
#### 4.2.3.3. Application Layer.
#### 4.2.3.4. Infrastructure Layer.
#### 4.2.3.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
    <img src="./resources/images/diagrams/../../diagrams/Transportation BC Component Diagram.png"     width ="700px" alt="Imagen" style="margin-right: 20px;">

</div>

#### 4.2.3.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.3.6.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.3.6.2. Bounded Context Database Design Diagram.


### 4.2.4. Bounded Context: Execution and tracking
#### 4.2.4.1. Domain Layer.
#### 4.2.4.2. Interface Layer.
#### 4.2.4.3. Application Layer.
#### 4.2.4.4. Infrastructure Layer.
#### 4.2.4.5. Bounded Context Software Architecture Component Level Diagrams.
#### 4.2.2.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.2.6.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.2.6.2. Bounded Context Database Design Diagram.


### 4.2.5. Bounded Context: Subscription and payment
#### 4.2.5.1. Domain Layer.
#### Entities:

* **Subscription**: Esta entidad representa una suscripción en el sistema. Tiene atributos como ID de suscripción, fecha de inicio, fecha de vencimiento y métodos para gestionar la suscripción, como renovarla o cancelarla.

* **Payment**: La entidad Payment modela los pagos realizados en el sistema. Contiene información sobre el ID de pago, el monto, la fecha y otros detalles relevantes. También incluye métodos para registrar y procesar pagos.

* **Insurance**: La entidad Insurance representa las pólizas de seguro disponibles en el sistema. Incluye atributos como el tipo de seguro, la cobertura y métodos para adquirir o administrar pólizas de seguro.

#### Object Values:

* **PaymentHistory**: Este object value almacena el historial de pagos asociado a una suscripción. Contiene detalles como las fechas de los pagos anteriores, el estado de los pagos y otros datos relacionados con el historial de pagos.

#### Aggregates:

* **SubscriptionAggregate**: Este aggregate agrupa la entidad de Suscripción (Subscription) y el historial de pagos (PaymentHistory) relacionado. Define las reglas de negocio que garantizan la consistencia entre suscripciones y pagos.

#### Enumeraciones:

* **PaymentStatus**: Esta enumeración representa el estado de un pago, incluyendo valores como "Procesado" o "Fallido". Se utiliza para rastrear el estado de los pagos en el sistema.

* **InsuranceType**: Enumeración que define los diferentes tipos de seguros disponibles.

#### 4.2.5.2. Interface Layer.

* **Payment Controller**: El controlador Payment maneja las solicitudes relacionadas con los pagos. Proporciona endpoints,registrar historiales de pagos y gestionar la interacción con los usuarios en términos de suscripciones y pagos.

* **Subscription Controller**: El controlador Subscription se encarga de las solicitudes relacionadas con las suscripciones. Ofrece endpoints para crear, renovar y cancelar suscripciones, así como para administrar el estado de las suscripciones de los usuarios.

* **Insurance Controller**: El controlador Insurance gestiona las interacciones relacionadas con las pólizas de seguro. Proporciona endpoints para adquirir, modificar y consultar información sobre las pólizas de seguro disponibles.


#### 4.2.5.3. Application Layer.


* **Purchase Subscription Command Handler**: Este Command Handler se encarga de procesar las solicitudes de compra de suscripciones. Recibe comandos de compra de suscripción desde el Interface Layer y coordina la creación y activación de las suscripciones en el Domain Layer. Además, gestiona la facturación y los registros de pagos relacionados con las suscripciones adquiridas.

* **Renew Subscription Command Handler**: El Command Handler de renovación de suscripciones maneja las solicitudes para extender la duración de una suscripción existente. Al recibir un comando de renovación de suscripción, este handler interactúa con el Domain Layer para actualizar las fechas de vencimiento y gestionar los pagos asociados a la renovación.

* **Adquire Insurance Command Handler**: Este Command Handler se encarga de procesar las solicitudes de adquisición de seguro. Cuando recibe un comando para adquirir un seguro, coordina la creación y configuración del seguro en el Domain Layer.

* **Payment Process Command Handler**: El Command Handler de procesamiento de pagos administra las solicitudes relacionadas con el procesamiento de pagos. Recibe comandos para procesar pagos y se comunica con el Domain Layer para registrar los pagos exitosos y gestionar los casos de pagos fallidos.


#### 4.2.5.4. Infrastructure Layer.

* **Subscription Repository**: Este repositorio se encarga de la persistencia de datos relacionados con las suscripciones de usuarios. Almacena información sobre las suscripciones activas, su estado y fechas de vencimiento. Facilita la consulta y actualización de datos de suscripciones.

* **Payment Gateway Adapter**: Este adaptador se conecta con un servicio externo de pasarela de pago mediante nuestro payment gateway.

* **Insurance Policy Repository**: Este repositorio maneja la persistencia de datos relacionados con los seguros adquiridos por los usuarios. Almacena información sobre los seguros activas, su cobertura y detalles relacionados con las pólizas.

* **Logging Service**: Proporciona registros para auditoría, seguimiento y resolución de problemas. Captura información sobre pagos procesados, interacciones de usuarios y eventos críticos.




#### 4.2.5.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
    <img src="./resources/images/diagrams/../../diagrams/Subscription and Payment BC Component Diagram.png"    width ="700px" alt="Imagen" style="margin-right: 20px;">

</div>

#### 4.2.5.6. Bounded Context Software Architecture Code Level Diagrams.


##### 4.2.5.6.1. Bounded Context Domain Layer Class Diagrams.
<div align="center">

<img src="/Resources/diagrams/subscriptionPayment.png" width="500px">

</div>

##### 4.2.5.6.2. Bounded Context Database Design Diagram.
<div align="center">

<img src="/Resources/diagrams/subscriptionPaymnetDB.png" width="500px">

</div>


### 4.2.6. Bounded Context: Review
#### 4.2.6.1. Domain Layer.
*  **Review** : representa una revisión o comentario que un turista deja sobre un paquete turístico ofrecido por una agencia de viajes.

*  **TourPackage** : La entidad representa un paquete turístico ofrecido por una agencia de viajes. Puede contener detalles sobre el destino, la duración del viaje, el precio y otros atributos relacionados con el paquete

*  **User** : Esta clase representa al usuario, teniendo como atributos el nombre de usuario, contraseña y un objeto de tipo Account.

### **Enum**:
* **Rol**: Esta clase representaría los diferentes tipos de usuarios en el sistema.
    * **Tourist**: representa a un turista o usuario que utiliza tu aplicación para buscar y reservar paquetes turísticos, así como para dejar revisiones.
    * **Agency**: son aquellos que ofrecen los paquetes turísticos o experiencias, tendrán privilegios y funcionalidades diferentes al user Tourist como la capacidad de crear y administrar paquetes turísticos, gestionar revisiones y otras acciones específicas de una agencia de viajes.
 

#### 4.2.6.2. Interface Layer.
* **Review Controller**: Este controlador es responsable de gestionar la interacción entre la interfaz de usuario y la lógica de negocio relacionada con las revisiones de paquetes turísticos en tu aplicación. Esto ayuda a mantener una separación clara de responsabilidades y a garantizar que la lógica de negocio se mantenga en la capa de aplicación, lo que facilita la escalabilidad y el mantenimiento de LifeTravel.

#### 4.2.6.3. Application Layer.
* **AddReview CommandHandler:** maneja el proceso de agregar una nueva revisión. Valida los datos del comando, realiza cálculos relacionados con la puntuación promedio y actualiza la base de datos con la nueva revisión.

* **UpdateReview CommandHandler:** Responsable de procesar la actualización de una revisión existente. Valida los datos del comando y actualiza la revisión correspondiente en la base de datos.

* **DeleteReview CommandHandler:** Maneja la eliminación de una revisión. Verifica que la revisión exista y la elimina de la base de datos.

#### 4.2.6.4. Infrastructure Layer.
* **Review Application Service:** actúa como un punto de entrada para las operaciones relacionadas con las revisiones de paquetes turísticos. Su función principal es coordinar las solicitudes desde la capa de aplicación y dirigirlas hacia los repositorios adecuados. Se comunica con los command Handler tanto para solicitudes de reviews como agregar o eliminar y autenticación y validación de roles.

* **User Repository:** es responsable de interactuar con la capa de almacenamiento o base de datos para realizar operaciones relacionadas con los usuarios

* **Review Repository:**  es responsable de interactuar con la capa de almacenamiento o base de datos para realizar operaciones relacionadas con las revisiones.

#### 4.2.6.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
    <img src="./resources/images/diagrams/../../diagrams/Review DC Component Diagram.png"     width ="700px" alt="Imagen" style="margin-right: 20px;">

</div>

#### 4.2.6.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.6.6.1. Bounded Context Domain Layer Class Diagrams.
<div align="center">

<img src="./resources/images/diagrams/../../diagrams/BC_Review_class.png" width="500px">

</div>

##### 4.2.6.6.2. Bounded Context Database Design Diagram.
<div align="center">

<img src="./resources/images/diagrams/../../diagrams/BC_Reviews_DB.png" width="500px">


| Campo             | Tipo                  | Descripción                                      |
|-------------------|-----------------------|--------------------------------------------------|
| review_id   | uniqueidentifier      | Identificador único de la reseña.         |
| tourist_id       | uniqueidentifier, FK      | Identificador único del turista.               |
| comment           | text         | Mensaje o descripción de la reseña.                     |
| tourPackage_id         | uniqueidentifier, FK                   | Identificador único del paquete turístico.  |
| stars              | int                   | cantidad de estrellas. |
| review_date           | datetime              | Fecha y hora de envío de la reseña.       |

</div>


### 4.2.7. Bounded Context: Notification
Mediante el uso de este bounded context se abordan las clases y capas relacionadas con las notificaciones hacia los usuarios por parte del sistema. A continuación, se detallan los principales componentes de este Bounded:
#### 4.2.7.1. Domain Layer.
*  **Notification** : Esta clase representa la notificación  que se enviara al usuario final, dentro de esta clase se encuentran atributos tales como : 
   - **message:** Este atributo representa el mensaje que será enviado al usuario
   -  **isEnable:** Este atributo representa un booleano, con este se puede saber si el usuario cuenta con las notificaciones activadas.
   -  **type:** Este atributo cuenta con los valores del enumerator **NotificationType**, representa que tipo de notificación  será enviada.
   -  **receiver:** Este atributo cuenta con los valores de la entidad **NotificationReceiver**, conteniendo la información necesaria para enviar la notificación  al usuario.
* **NotificationReceiver:** Esta clase representa el modelo que es necesario para poder obtener la información necesaria para enviar la notificación al usuario, como atributos tiene:
    - **name:** Atributo que representa el nombre del usuario al que se le enviara la notificación.
    - **email:** Correo al que se le enviara la notificación en caso sea necesario. 
### **Enum**:
* **NotificationType**: Representa el tipo de notificación  que será enviada. Los tipos de notificaciones son los siguientes : 
    - **WEATHER :**     Representa las notificaciones de tipo **Alerta de clima** 
    - **CLOTHING**      Representa las recomendaciones de vestimenta para el tour
    - **RESERVATION:** Representa las notificaciones referentes a las reservas de los tours
    - **REGISTRATION:** Son las notificaciones del registro, estas serán enviadas por email

#### 4.2.7.2. Interface Layer.
* **Notification Controller:** Este controlador maneja las solicitudes relacionadas con las notificaciones vía correo y notificaciones móviles. Además, recopila los datos para luego almacenarlos en la base de datos.
  
#### 4.2.7.3. Application Layer.


- **WeatherNotificationCommandHandler:** Este CommandHandler se encarga de enviar notificaciones de alerta de clima **(NotificationType.WEATHER)** al usuario final.

- **ClothingNotificationCommandHandler:** Este CommandHandler gestiona las notificaciones de recomendaciones de vestimenta **(NotificationType.CLOTHING)**.

- **ReservationNotificationCommandHandler:** Este CommandHandler maneja las notificaciones relacionadas con las reservas de tours **(NotificationType.RESERVATION)**.

- **RegistrationNotificationCommandHandler:** Este CommandHandler se encarga de enviar notificaciones por correo electrónico del registro **(NotificationType.REGISTRATION)** al usuario final.

#### 4.2.7.4. Infrastructure Layer.
- **Notification Service:** Este servicio se encarga de gestionar el envío de notificaciones a través de diferentes canales, como correo electrónico o notificaciones móviles. Implementa la lógica para entregar las notificaciones al usuario final según las preferencias y la elección del canal.
- **Notification Repository** El repositorio de notificaciones almacena y gestiona las notificaciones enviadas. Esto incluye el seguimiento de qué notificaciones se han enviado, cuándo se enviaron y a quién se enviaron. Además, permite realizar consultas y búsquedas relacionadas con el historial de notificaciones.
  
  <hr>
#### 4.2.7.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
    <img src="https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/Notification%20DC%20Component%20Diagram.png?raw=true"     width ="700px" alt="Imagen" style="margin-right: 20px;">

</div>

#### 4.2.7.6. Bounded Context Software Architecture Code Level Diagrams.

##### 4.2.7.6.1. Bounded Context Domain Layer Class Diagrams.

<div align="center">

<img src="https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/BC_Notification_class.png?raw=true" width="500px">

</div>

##### 4.2.7.6.2. Bounded Context Database Design Diagram.

Para este bounded context, definimos que la clase encargada sea la siguiente :

<div align="center">
    <img src= "https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/BC_Notificactions_DB.png?raw=true" width="400px">
</div>



<hr>

| Campo             | Tipo                  | Descripción                                      |
|-------------------|-----------------------|--------------------------------------------------|
| notification_id   | uniqueidentifier      | Identificador único de la notificación.         |
| receiver_id       | uniqueidentifier, FK      | Identificador único del receptor.               |
| message           | nvarchar(max)         | Mensaje de la notificación.                     |
| is_enabled        | bit                   | Indica si las notificaciones están habilitadas.  |
| type              | int                   | Tipo de notificación (WEATHER = 1, CLOTHING = 2, RESERVATION = 3, REGISTRATION = 4). |
| sent_at           | datetime              | Fecha y hora de envío de la notificación.       |
| delivery_method   | nvarchar(max)         | Medio de entrega de la notificación (EMAIL, MOBILE_APP, OTRO). |



### 4.2.8. Bounded Context: Identity and Access
Mediante el uso de este bounded context se abordan las clases y capas relacionadas con la identidad y el acceso de los usuarios al sistema. A continuación, se detallan las principales componentes de este contexto:

#### 4.2.8.1. Domain Layer.
*  **User** : Esta clase representa al usuario, teniendo como atributos el nombre de usuario, contraseña y un objeto de tipo Account. Tendría métodos para poder cerrar la cuenta y también para determinar si el usuario es dueño de la cuenta.
* **Account**: Esta clase representa la cuenta conectada al usuario, teniendo como atributos el nombre de usuario, un identificador, un objeto owner de tipo User y un rol para especificar a qué segmento objetivo pertenece. Entre sus métodos se encuentran cambiar el tipo de suscripción, crear un usuario, entre otros.
### **Enum**:
* **Rol**: Esta clase representaría los diferentes tipos de usuarios en el sistema.




#### 4.2.8.2. Interface Layer.
* **SignIn Controller**: Este controlador maneja las solicitudes relacionadas con la autenticación e inicio de sesión de los usuarios. Permite el inicio de sesión y la gestión de cuentas de usuario existentes en la plataforma. Utiliza Firebase Authentication para la autenticación de usuarios.

* **SignUp Controller** :  Este controlador se encarga de las solicitudes de creación de nuevas cuentas de usuario. Facilita el registro de nuevos usuarios en la plataforma mediante Firebase Authentication.


#### 4.2.8.3. Application Layer.

* **SignIn CommandHandler:** Este comando se encarga de manejar las solicitudes de inicio de sesión de usuarios en el sistema. Cuando recibe una solicitud de inicio de sesión del SignIn Controller, verifica las credenciales utilizando Firebase Authentication y permite o deniega el acceso según el resultado.

* **SignUp CommandHandler:** Se encarga de gestionar las solicitudes de creación de nuevas cuentas de usuario en la plataforma. Cuando recibe una solicitud de registro del SignUp Controller, utiliza Firebase Authentication para registrar al nuevo usuario y, si la operación tiene éxito, crea una cuenta de usuario en la base de datos.
* **Account Reporting CommandHandler:** Este Command Handler se encarga de procesar las solicitudes de reporte de cuentas de usuario.

<div align="center" >
    <img src="https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/hanlders.png?raw=true"     width ="250px" alt="Imagen" style="margin-right: 20px;">
</div>

#### 4.2.8.4. Infrastructure Layer.

* **SignUp Application Service:** Este componente es parte de la capa de infraestructura y se encarga de gestionar la lógica de aplicación relacionada con el registro de usuarios. Trabaja en conjunto con el SignUp CommandHandler para crear nuevas cuentas de usuario utilizando Firebase Authentication. Además, puede estar conectado a la base de datos para almacenar información adicional sobre los usuarios registrados.
* **SignIn Application Service:** Se encarga de gestionar la lógica de aplicación relacionada con el inicio de sesión de usuarios. Colabora con el SignIn CommandHandler para autenticar a los usuarios utilizando Firebase Authentication.
* **User Repository:**  Su principal función es interactuar con la base de datos para realizar operaciones de lectura y escritura de información de usuarios. Almacena y recupera datos de usuarios, como perfiles, credenciales y roles.
* **FireBase Adapter:** Se encarga de comunicarse con Firebase Authentication para realizar operaciones como el registro y el inicio de sesión de usuarios. 
  


#### 4.2.8.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
    <img src="https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/Identity%20and%20Access%20DC%20Component%20Diagram.png?raw=true"    width ="700px" alt="Imagen" style="margin-right: 20px;">

</div>

#### 4.2.8.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.8.6.1. Bounded Context Domain Layer Class Diagrams.

<div align="center" >
    <img src="https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/profile.png?raw=true"     width ="250px" alt="Imagen" style="margin-right: 20px;">
</div>

##### 4.2.8.6.2. Bounded Context Database Design Diagram.



### 4.2.9. Bounded Context: Booking 
### 4.2.9. Bounded Context: Booking
Este bounded context se enfoca en las clases y capas relacionadas con la gestión de reservas de tours por parte de los usuarios viajeros y la administración de estas reservas por parte de las agencias de viaje. A continuación, se detallan las principales componentes de este contexto:
#### 4.2.9.1. Domain Layer.
- **Tour:** Esta clase representa un tour que los usuarios pueden reservar. Contiene atributos como nombre del tour, descripción, precio, fecha y ubicación. Puede incluir métodos para verificar la disponibilidad de fechas y gestionar las reservas.
- **Booking:** Esta clase representa una reserva de un usuario para un tour específico. Contiene información sobre el usuario que realiza la reserva, el tour reservado, la fecha de la reserva y otros detalles relevantes.
- **Agency:** Esta clase representa una agencia de viaje que ofrece tours. Contiene información sobre la agencia, como nombre, dirección, y lista de tours que ofrece.


*Enum:*
- **BookingStatus:** Este enum define los posibles estados de una reserva, como pendiente, confirmada o cancelada.
- **PaymentStatus:** Este enum define los posibles estados de pago para una reserva, como pagado o pendiente de pago.
#### 4.2.9.2. Interface Layer.
- **BookingController:** Este controlador maneja las solicitudes relacionadas con la reserva de tours por parte de los usuarios viajeros. Permite a los usuarios buscar tours disponibles, seleccionar fechas y realizar reservas.




#### 4.2.9.3. Application Layer.
- **BookingApplicationService:** Este servicio de aplicación se encarga de procesar las solicitudes de reserva de tours por parte de los usuarios viajeros. Verifica la disponibilidad de fechas, crea las reservas y gestiona los pagos.


#### 4.2.9.4. Infrastructure Layer.
- **TourPackageRepository:** Su función principal es interactuar con la base de datos para realizar operaciones de lectura y escritura de información sobre tours. Almacena y recupera datos de tours, fechas disponibles y detalles de reserva.
- **BookingRepository:** Almacena y recupera información sobre las reservas realizadas por los usuarios viajeros, incluyendo detalles de usuario, tour, fechas y estados de reserva.
- **EmailService:** Puede ser responsable de enviar confirmaciones de reserva y notificaciones relacionadas con las reservas a los usuarios y las agencias de viaje.
- **VehicleRepository:**  Interactúa con la base de datos para realizar operaciones de lectura y escritura de información sobre vehículos utilizados en los tours. Almacena y recupera datos sobre los vehículos disponibles para los tours.
- **Notification Repository:** Almacena y recupera información sobre las notificaciones relacionadas con las reservas, como confirmaciones, cambios de estado y recordatorios de tours.
#### 4.2.9.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
   <img src="https://github.com/NexusNova-IOT/upc-pre-202302-si572-SW71-nexusnova-report/blob/tb1/Resources/diagrams/Booking%20BC%20Component%20Diagram.png?raw=true"    width ="700px" alt="Imagen" style="margin-right: 20px;">
</div>


#### 4.2.9.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.9.6.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.9.6.2. Bounded Context Database Design Diagram.


</div>

### 4.2.10. Bounded Context: IoT Asset Management  
#### 4.2.10.1. Domain Layer.
*  **IoTDevice** : Esta clase representa un dispositivo IoT genérico y actúa como una entidad padre para varios tipos de dispositivos IoT teniendo como atibutos IP  y MAC address.
    * **Scale**: Clase hija que representa una balanza IoT utilizada en el negocio para poder gestionar el peso adecuado por unidad terrestre destinada a la experiencia turística.
    * **WeatherSensor**: Esta clase representa un sensor IoT utilizado para medir datos climáticos con principales funciones como registrar y mantener información específica del sensor climático. Proporcionar métodos para tomar mediciones climáticas y obtener datos relacionados con el clima.
    * **LocalizationWristband**: Esta clase representa una pulsera de localización IoT utilizada para rastrear la ubicación de los turistas. 

#### 4.2.10.2. Interface Layer.
* **Scale Controller**: Es responsable de gestionar las solicitudes y las interacciones relacionadas con la balanza  como coordinar con la Application Layer para ejecutar operaciones específicas en las balanzas, como tomar mediciones de peso y registrar datos.

* **Weather Sensor Controller** :  Se encarga de gestionar las solicitudes y las operaciones relacionadas con los sensores climáticos IoT como validar los datos de entrada relacionados con los sensores climáticos y coordinar con la capa de aplicación para obtener datos climáticos específicos de los sensores.

* **Localization Wristband Controller** :  Se encarga de gestionar las solicitudes y las operaciones relacionadas con las pulseras de localización.


#### 4.2.10.3. Application Layer.
* **Scale CommandHandler:** Este command handler se encarga de procesar comandos relacionados con las balanzas IoT, como comandos para realizar mediciones de peso, calibración de balanzas, etc.

* **WeatherSensor CommandHandler:** Este handler procesa comandos relacionados con los sensores climáticos IoT, como comandos para obtener mediciones de temperatura, humedad, etc. Cuando se recibe un comando relacionado con sensores climáticos, este handler toma las mediciones correspondientes, las valida y actualiza el estado de los sensores climáticos en la capa de dominio.

* **LocalizationWristband CommandHandler:** se encarga de procesar comandos relacionados con las pulseras de localización IoT, como comandos para obtener la ubicación actual de una pulsera, actualizar configuraciones, etc.


#### 4.2.10.4. Infrastructure Layer.
* **IoT Asset Scale Application Service:** Este servicio de aplicación se encarga de coordinar las operaciones relacionadas con las balanzas IoT. Recibe las consultas de la capa de aplicacion y las valida para que pueda interactuar con el scale repository.
* **IoT Asset Weather Sensor Application Service:**  Recibe solicitudes relacionadas con sensores climáticos desde la capa de interfaz o la capa de aplicación. Asimismo, valida y procesa estas solicitudes, garantizando que se cumplan las reglas de negocio y la lógica específica de los sensores climáticos.
* **IoT Asset Tracking Application Service:** Coordina las operaciones relacionadas a las pulseras de localizacion que usan los turistas durante la experiencia. Nos brinda una conexion con el Repository para que se puede acceder y actualizar datos que las pulseras almacenan en la base de datos.
* **Scale Repository:**  Almacena y recupera información sobre las balanzas IoT, incluyendo su estado, configuración y mediciones registradas.
* **Weather Sensor Repository:** Almacena y recupera datos de los sensores climáticos, como mediciones de temperatura, humedad, etc.
* **Localization Wristband Repository:** Es el repository, encargado de almacenar y recuperar datos relacionados con la localizacion de las pulseras, como la ubicacion, estado de la pulsera, donde esta asigna, etc. 

#### 4.2.10.5. Bounded Context Software Architecture Component Level Diagrams.
<div style="display: flex; align-items: center;">
    <img src=""
    width ="700px" alt="Imagen" style="margin-right: 20px;">
</div>

#### 4.2.10.6. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.10.6.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.10.6.2. Bounded Context Database Design Diagram.