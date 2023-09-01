## 4.1. Strategic-Level Domain-Driven Design

En el siguiente apartado, se detalla una serie de enfoques clave en el proceso de Diseño Dirigido por el Dominio a nivel estratégico (Strategic-Level Domain-Driven Design). Estos enfoques desempeñaron un papel fundamental en el establecimiento de una base sólida para la definición y modelado de dominios complejos. A través de técnicas como Event Storming, Context Mapping y la definición de la Arquitectura de Software, se logró obtener una comprensión profunda de los elementos esenciales necesarios para la creación de sistemas efectivos y bien estructurados. A continuación, se describen los puntos clave que se abordaron en esta sección.

### 4.1.1. EventStorming

Se abordó un enfoque colaborativo y visual que permitió modelar el contexto del dominio. Se exploraron las etapas de Candidate Context Discovery, Domain Message Flows Modeling y la creación de Bounded Context Canvases.

#### 4.1.1.1 Candidate Context Discovery.
#### 4.1.1.2 Domain Message Flows Modeling.
#### 4.1.1.3 Bounded Context Canvases.

### 4.1.2. Context Mapping

Se analizó una técnica que resultó invaluable para gestionar las interacciones y límites entre diferentes contextos del dominio. Se exploró cómo mapear y definir relaciones entre contextos, lo que contribuyó a una comprensión clara de sus interconexiones.

### 4.1.3. Software Architecture

Se presentaron diversas perspectivas arquitectónicas que ayudaron a visualizar y estructurar sistemas de software. Se exploraron diagramas a nivel de Paisaje del Sistema, Nivel de Contexto y Nivel de Contenedor, así como Diagramas de Despliegue que arrojaron luz sobre la infraestructura en la que operaría el sistema.

#### 4.1.3.1. Software Architecture System Landscape Diagram.
#### 4.1.3.2. Software Architecture Context Level Diagrams.
#### 4.1.3.2. Software Architecture Container Level Diagrams.
#### 4.1.3.3. Software Architecture Deployment Diagrams.


## 4.2. Tactical-Level Domain-Driven Design
### 4.2.1. Bounded Context: Profile management
En esta sección, presentaremos la propuesta táctica para el diseño de la solución de software en el contexto de "Profile Management". Detallaremos las clases identificadas y explicaremos sus atributos, métodos y relaciones, siguiendo una estructura que abarca las diferentes capas de nuestra arquitectura.
#### 4.2.1.1. Domain Layer.

#### 4.2.1.2. Interface Layer.
#### 4.2.1.3. Application Layer.
#### 4.2.1.4. Infrastructure Layer.
#### 4.2.1.6. Bounded Context Software Architecture Component Level Diagrams.
#### 4.2.1.7. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.1.7.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.1.7.2. Bounded Context Database Design Diagram.


### 4.2.2. Bounded Context: Tour Experience
#### 4.2.2.1. Domain Layer.
#### 4.2.2.2. Interface Layer.
#### 4.2.2.3. Application Layer.
#### 4.2.2.4. Infrastructure Layer.
#### 4.2.2.6. Bounded Context Software Architecture Component Level Diagrams.
#### 4.2.2.7. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.2.7.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.2.7.2. Bounded Context Database Design Diagram.


### 4.2.3. Bounded Context: Transport management
#### 4.2.3.1. Domain Layer.
#### 4.2.3.2. Interface Layer.
#### 4.2.3.3. Application Layer.
#### 4.2.3.4. Infrastructure Layer.
#### 4.2.3.6. Bounded Context Software Architecture Component Level Diagrams.
#### 4.2.3.7. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.3.7.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.3.7.2. Bounded Context Database Design Diagram.


### 4.2.4. Bounded Context: Execution and tracking
#### 4.2.4.1. Domain Layer.
#### 4.2.4.2. Interface Layer.
#### 4.2.4.3. Application Layer.
#### 4.2.4.4. Infrastructure Layer.
#### 4.2.4.6. Bounded Context Software Architecture Component Level Diagrams.
#### 4.2.2.7. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.2.7.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.2.7.2. Bounded Context Database Design Diagram.


### 4.2.5. Bounded Context: Subscription and payment
#### 4.2.5.1. Domain Layer.
En la capa de dominio de "Subscription and Payment", se definen clases esenciales para modelar las suscripciones y los pagos. Estas clases están organizadas en categorías clave:
## Entities
- **Subscription**: Representa una suscripción activa con detalles como duración y tipo de servicio. Puede incluir lógica para renovaciones.
## Value Objects
- **ServiceType**: Define categorías de servicios como "Plan Urpi" o "Plan Tunki".

## Aggregates
- **UserAggregate**: Agrupa entidades y objetos de valor para usuarios, incluyendo sus suscripciones y pagos.

## Factories
- **SubscriptionFactory**: Crea instancias de suscripciones con reglas específicas.
- **PaymentFactory**: Crea pagos y asegura procesos adecuados.

## Domain Services
- **SubscriptionValidationService**: Valida suscripciones y condiciones.
- **PaymentGatewayService**: Procesa transacciones financieras.

## Repositories
- **SubscriptionRepository**: Persiste y recupera información de suscripciones.
- **PaymentRepository**: Maneja almacenamiento de pagos.

## Interfaces 
- **SubscriptionRepository**: Definición de métodos para acceder a las suscripciones.
- **PaymentRepository**: Definición de métodos para acceder a los pagos.

#### 4.2.5.2. Interface Layer.
#### 4.2.5.3. Application Layer.
#### 4.2.5.4. Infrastructure Layer.
#### 4.2.5.6. Bounded Context Software Architecture Component Level Diagrams.
#### 4.2.5.7. Bounded Context Software Architecture Code Level Diagrams.
##### 4.2.5.7.1. Bounded Context Domain Layer Class Diagrams.
##### 4.2.5.7.2. Bounded Context Database Design Diagram.