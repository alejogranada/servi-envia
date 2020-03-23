# servi-envia
Una compañía de Envíos (Servi-Envía), ubicada en la ciudad de Manizales, desea mejorar su Sistema Web, tanto en comunicación y arquitectura de Software para permitir ampliar su portafolio de Clientes y la forma de acceso de los mismos al sistema. Adicional, permitiendo facilidad en su manejo y promoción a ser multiplataforma. Servi-Envía pretende mejorar requerimientos de clientes y así interactuar con ellos de una manera más personalizada, optimizando a su vez el tiempo de atención entre las solicitudes de dichos clientes.
Siguiendo los lineamientos de este propósito para la organización, se debe construir un sistema orientado en la Arquitectura SOA, que implemente las siguientes funcionalidades:

− Registrar nuevo cliente en el sistema. Los datos a tener en cuenta son:

	o Cédula
	o Nombres
	o Apellidos
	o Fecha de nacimiento
	o Lugar de residencia
	o Teléfono
	o Correo electrónico
	o Fecha de registro Sistema
	o Estado (activo/inactivo – True/False)
	o Si el cliente ya estaba registrado mostrar un mensaje
	correspondiente.

− Buscar un cliente almacenado en el sistema:

	o Si se encuentra coincidencia de cliente, mostrar algunos datos
	relevantes de este.
	o Si no existe el cliente mostrar un mensaje correspondiente.

− Modificar datos del cliente.

− Permitir cambiar el estado de un cliente.

− Registrar envío de Mercancía. Los datos a tener en cuenta son:

	o Cédula cliente (quién envía – Emisor)
	o Cédula destinatario (quién recibe – Receptor)
	o Nombres destinatario
	o Apellidos destinatario
	o Ciudad origen
	o Ciudad destino
	o Peso paquete (Kl)
	o Valor asegurado
	o Valor envío (autocalculado)
	o Este valor autocalculado se dará como respuesta de la solicitud y con su correspondiente número de guía. 
		Se sugiere tener una tabla donde se encuentre almacenado el valor a pagar x Kl. según ciudad de Origen y Destino. 
		Dicho valor es el resultado de:
		
		Precio Kl = Según Origen y Destino (Se obtiene de una tabla en BD)
		Peso = Peso total del paquete que se envía (Se recibe en la solicitud)
		Seguro = Valor asegurado para la mercancía (Se recibe en la solicitud)
		𝑥 = (𝑃𝑟𝑒𝑐𝑖𝑜 𝐾𝑙 × 𝑃𝑒𝑠𝑜) + (𝑆𝑒𝑔𝑢𝑟𝑜 × 20%)

− Permitir cambio de estado en el que se encuentra un paquete enviado. 

	  o Teniendo en cuenta el número de guía se puede asignar/cambiar el estado de un paquete.
	  o Los posibles estados:

	    ▪ Pendiente (estado inicial para todos los paquetes que se
	    envían)
	    ▪ Recolectado (cuando el camión recoge el paquete en oficina)
	    ▪ Enviado (cuando se está transportando la mercancía)
	    ▪ Entregado (cuando el destinatario ha recibido su paquete)

− Consultar estado de una guía.


Para este propósito se ve la posibilidad de contar con la ayuda de 2 Especialistas en Desarrollo de Software que puedan resolver dicho aplicativo, teniendo en cuenta:


	• Se debe realizar un sistema funcional en modo Web Service mediante la
	tecnología ASMX, WCF ó Web API en .NET.

	• Usando Base de Datos SQL Server para guardar/consultar los datos.

	• El servicio debe estar desplegado en un Entorno Cloud (SaaS).

	• Implementación de cliente, que pueda consumir dicho servicio: App.
	Escritorio - App. Consola - App. Web - App. Móvil, en cualquier lenguaje de
	programación (Java, Python, PHP, Android, C#, Visual Basic, JSP, etc.).

	• Enviar documentación de Manual de usuario con lo realizado (servicio y
	cliente).

	• Incluir enlace dónde se encuentra alojado el Web Service.

	• Adjuntar binarios del Servicio y de la App. Cliente.

	• Enviar Scripts de BD Full (Creación de BD, Tablas y sus datos).

	• Adjuntar un corto video con el aplicativo funcionando, servicio recibiendo
	peticiones y BD con registros.
