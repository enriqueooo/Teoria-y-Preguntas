## Patrones de Diseño para la Comunicación entre Componentes.

# Teoría
Para empezar, los patrones de diseño son soluciones reutilizables y probadas para problemas comunes que enfrentamos al diseñar software. Estos patrones nos ayudan a resolver problemas de manera eficiente y facilitan el mantenimiento del código. Hoy nos enfocaremos en tres patrones clave que facilitan la comunicación entre componentes: el patrón de Observador, el patrón de Mediador y el patrón de Publicación/Suscripción.

Patrón de Observador (Observer Pattern):

Este patrón permite que un objeto (el sujeto) notifique a otros objetos (los observadores) sobre cambios en su estado sin tener que conocer los detalles internos de esos objetos.
Es útil en sistemas donde necesitamos mantener la consistencia del estado entre diferentes componentes. Por ejemplo, en una aplicación de bolsa de valores, cuando cambia el precio de una acción, todos los gráficos y tablas relacionados deben actualizarse automáticamente.
Patrón de Mediador (Mediator Pattern):

Este patrón centraliza la comunicación entre componentes para reducir las dependencias directas entre ellos.
Imagina un aeropuerto donde el control del tráfico aéreo (el mediador) coordina los despegues y aterrizajes de los aviones, evitando así que los aviones necesiten comunicarse directamente entre sí.
Patrón de Publicación/Suscripción (Publish/Subscribe Pattern):

Este patrón permite que los componentes se comuniquen de manera desacoplada mediante la definición de eventos a los que los componentes pueden suscribirse o publicar.
Es ideal para sistemas donde los componentes deben reaccionar a eventos específicos de manera asíncrona. Piensa en una aplicación de noticias donde un servicio publica noticias y los usuarios suscritos reciben actualizaciones automáticamente.
# Reflexión
Implementar estos patrones puede cambiar radicalmente cómo interactúan los componentes en nuestro sistema, promoviendo un diseño más modular y flexible. Reducimos la complejidad de las interacciones y mejoramos la mantenibilidad del código. Sin embargo, es crucial elegir el patrón adecuado para el problema específico, ya que una mala elección podría agregar una sobrecarga innecesaria o complejidad adicional.

# Analogía
Para entender mejor estos patrones, pensemos en una casa inteligente.

El patrón de Observador es como una luz que se enciende automáticamente cuando detecta movimiento, notificando a otros dispositivos como cámaras de seguridad o sistemas de alarma.
El patrón de Mediador es como un panel de control central que coordina la interacción entre el termostato, las luces y las cerraduras de las puertas, asegurando que todo funcione en armonía sin necesidad de comunicación directa entre los dispositivos.
El patrón de Publicación/Suscripción es como un sistema de alerta de seguridad, donde múltiples dispositivos (como sensores de puerta y cámaras) publican eventos a los que otros dispositivos de seguridad (como alarmas o notificaciones en smartphones) están suscritos y reaccionan en consecuencia.
Resumen
En resumen, los patrones de diseño son esenciales para gestionar la comunicación entre componentes de manera eficiente. El patrón de Observador, el patrón de Mediador y el patrón de Publicación/Suscripción nos ofrecen soluciones específicas para diferentes tipos de interacción, mejorando la modularidad y flexibilidad de nuestro código. Debemos seleccionar el patrón adecuado basándonos en un análisis cuidadoso de nuestras necesidades y la arquitectura del sistema.

# Referenciado de libros
Gamma, E., Helm, R., Johnson, R., & Vlissides, J. (1994). Design Patterns: Elements of Reusable Object-Oriented Software. Addison-Wesley.
Freeman, E., & Robson, E. (2004). Head First Design Patterns. O'Reilly Media.
Fowler, M. (2002). Patterns of Enterprise Application Architecture. Addison-Wesley.