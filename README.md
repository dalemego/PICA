# PICA
Proyecto de implementacion centrado en la arquitectura

# Atributos de calidad 
 
## Robustez: 
El sistema debe tener la capacidad de ser modificado fácilmente con el fin de no afectar la alta disponibilidad requerida por el negocio. Para esto nos enfocamos en un modelo FaaS con el fin de implementar una arquitectura basada en contenedores que permita la ejecución independiente de sus componentes.
 
## Rendimiento: 
El uso de contenedores tendrá como ventaja un impacto positivo en el rendimiento del sistema, permitiendo ajustar cada componente  para su ejecución optima. Además, la inclusión de componentes como Kafka dentro de la arquitectura de microservicios, permite la gestión de un alto flujo de datos para un mejor rendimiento general del sistema.
 
## Integridad y no repudio: 
Se debe hacer énfasis en la confiabilidad e integridad de la información, al ser compartida con otros servicios como también garantizarse la integridad transaccional a lo largo del flujo del pedido de lado del cliente, por lo que el uso de sagas dentro de la implementación garantiza que cada transacción sea integra desde su inicio hasta la respuesta final al cliente.
 
## Interoperabilidad: 
El servicio debe ser capaz de intercambiar correctamente la información con otros componentes del sistema. De nuevo el uso de contenedores nos da la facilidad de que cada uno de los microservicios sea independiente pero que a su vez pueda ejecutarse utilizando información de otros componentes de manera eficaz.
 
## Escalabilidad: 
A medida que TouresBalón acepte medios de pago adicionales se aumentará el volumen de usuarios en la plataforma, por lo tanto, es importante que el sistema permitá la escalabilidad de los diferentes módulos de manera que cualquier adición a la arquitectura conviva con la implementación existente sin requerir un rediseño total de la arquitectura base. 

