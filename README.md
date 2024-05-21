![image](https://github.com/mateommarulanda/serviciocorreo/assets/60433396/a4fe1d72-107c-4040-bfb6-248e6a0f8eb1)

Explicación del diagrama:
•	La interfaz IServicioCorreo define las funcionalidades del servicio de correo.
•	La clase ServicioCorreo implementa la interfaz IServicioCorreo.
•	La clase EnvioCorreo es responsable de enviar correos electrónicos.
•	La clase ListadoCorreos es responsable de listar los correos electrónicos.
•	La clase DescargaCorreo es responsable de descargar los correos electrónicos.
•	La clase ConfiguracionCorreo es responsable de almacenar la configuración del servicio de correo.
•	La clase GestorEventos es responsable de registrar los eventos que ocurren con el servicio.
•	La clase CacheCorreo es responsable de almacenar en caché los resultados de las operaciones del servicio.

Decisiones de diseño:

Se ha utilizado el patrón de diseño Decorador para extender la funcionalidad de la clase ServicioCorreo. Esto permite agregar nuevas funcionalidades al servicio sin modificar la clase original.
Se ha utilizado el patrón de diseño Estrategia para implementar el reintento de las solicitudes fallidas. Esto permite cambiar la estrategia de reintento sin modificar la clase EnvioCorreo.
Se ha utilizado el patrón de diseño Singleton para implementar la clase GestorEventos. Esto garantiza que solo haya una instancia de la clase GestorEventos en el sistema.
Se ha utilizado el patrón de diseño Memento para implementar la clase ConfiguracionCorreo. Esto permite guardar y restaurar la configuración del servicio de correo.

Patrones de diseño
Los siguientes patrones de diseño se han utilizado en la solución propuesta:

Patrón Decorador: Este patrón se utiliza para extender la funcionalidad de una clase existente sin modificar la clase original. En este caso, se utiliza para agregar nuevas funcionalidades al servicio de correo, como el reintento de solicitudes fallidas y el registro de eventos.
Patrón Estrategia: Este patrón se utiliza para definir una familia de algoritmos, encapsular cada uno de ellos y hacer que sean intercambiables. En este caso, se utiliza para implementar el reintento de las solicitudes fallidas.
Patrón Singleton: Este patrón se utiliza para garantizar que solo haya una instancia de una clase en el sistema. En este caso, se utiliza para implementar la clase GestorEventos.
Patrón Memento: Este patrón se utiliza para guardar y restaurar el estado de un objeto. En este caso, se utiliza para implementar la clase ConfiguracionCorreo.
