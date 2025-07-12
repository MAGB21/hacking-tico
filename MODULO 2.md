## 2.1
### regulaciones
1. PCI DSS (Regulación del Estándar de seguridad de datos de la industria de pagos)
	1. Tiene como objetivo proteger el procesamiento de los pagos con tarjeta de crédito y otros tipos de pagos digitales.
2. HIPAA (Ley de portabilidad y responsabilidad de los Seguro de Salud )
	1. Sirve para simplificar y estandarizar los procesos administrativos de los servicios de salud
3. FedRAMP
	1. Su propósito es automatizar el uso de las ofertas de servicios en la nube

## CONCEPTOS LEGALES
1. Acuerdo de nivel de servicio (SLA)
	1. Un SLA es una expectativa o restricción bien documentada relacionada con una o más de las medidas de rendimiento mínimas o máximas tales como.
		1. Calidad
		2. Línea de tiempo 
		3. plazo y costo
2. Confidencialidad
	1. Debe analizar y acordar el manejo de datos confidenciales. por ejemplo,si puede encontrar contraseñas u otros datos confidenciales debería hacerse preguntas tales como:.
		1. ¿Necesita divulgar todas esas contraseñas o todos esos datos confidenciales?
		2. ¿Quién tendrá acceso a los datos confidenciales?
		3. ¿Cuál será la forma correcta de comunicar y manejar dichos datos?
		De manera similar, debe proteger los datos confidenciales y eliminar todos los registros, según su acuerdo con su cliente.
3. Declaración de trabajo (SOW)
	1. un SOW un documento que especifica las actividades que se realizarán durante un compromiso de prueba de penetración. se puede utilizar para definir algunos de los siguientes elementos:
		1. Líneas de tiempo del proyecto(Pruebas de penetración), incluido el cronograma de entrega de informes.
		2. El alcance del trabajo a realizar.
		3. La ubicación del trabajo (ubicación geográfica o ubicación de red)
		4. Requisitos técnicos y no técnicos especiales
		5. Calendario de pagos
		6. Elementos varios que puedes no ser parte de la negociación principal, pero que deben enumerarse y rastrearse porque podrían plantear problemas durante la interacción general
		**Nota el SOW puede ser un documento independiente o puede ser parte de un acuerdo de servicio maestro(MSA)**
4. Acuerdo de servicio maestro
	1. Los MSA, que son muy populares en la actualidad, son contratos que se pueden utilizar para negociar rápidamente el trabajo que se realizará, además son beneficiosos porque estos pueden ser guardados para cuando se requiera hacer una nueva prueba de penetración no se tenga que hacer todo el documento desde cero y se verifique que hayan hecho ya las correcciones previas a dichos ataques, además de hacer pruebas en otras áreas de la empresa
5. Acuerdo de no divulgación (NDA)
	1. Un NDA es un documento legal y un contrato entre usted y una organización que lo ha contratado como evaluador de penetración. Un NDA especifica y define material, conocimiento e información confidencial que no debe divulgarse y que ambas partes deben mantener confidencial.
	2. los NDA se clasifican en la siguiente manera:
		1. Unilateral
				Con una NDA unilateral, solo una parte divulga cierta información a la otra parte, la información debe mantenerse protegida y no divulgada. Por ejemplo, una organización que le contrata debe incluir en un NDA determinada información que no debe divulgar. Por supuesto, todos sus hallazgos deben mantenerse en secreto y no deben revelarse a ninguna otra organización o individuo
		2. Bilateral
				Un NDA bilateral también se denomina NDA mutuo o bidireccional, donde ambas partes comparten información confidencial entre si y esta información no debe revelarse a ninguna otra entidad
		3. Multilateral
				Este tipo de NDA involucra a tres o más partes, y al menos una de las partes divulga información confidencial que no debe revelarse a ninguna entidad fuera del acuerdo.
## 2.2
### 2.2.2 Reglas de compromiso
existe un documento donde se definen las reglas de participación y en este mismo se especifican las condiciones en las que se realizará la participación de pruebas de penetración de seguridad.
elementos que normalmente se incluyen en el documento:
1.-

| Elementos de regla de participación                                                 | ejemplo                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ----------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| pruebas de línea de tiempo (uso de diagramas de Gantt)                              | Tres semanas, como se especifica en un dialogo                                                                                                                                                                                                                                                                                                                                                                               |
| Ubicación de la prueba                                                              | Sede de la empresa en Raleigh, Carolina del Norte                                                                                                                                                                                                                                                                                                                                                                            |
| Ventana de tiempo de la prueba (horas del día)                                      | de 8:00 a.m a 5:00p.m hora del este de los Estados Unidos                                                                                                                                                                                                                                                                                                                                                                    |
| Método de comunicación preferido                                                    | Informe final y reuniones semanales de actualización de estado                                                                                                                                                                                                                                                                                                                                                               |
| Los controles de seguridad que potencialmente podrían detectar o evitar las pruebas | Sistemas de prevención de intrusiones (IPS), cortafuegos, sistemas de prevención de pérdida de datos (DLP)                                                                                                                                                                                                                                                                                                                   |
| Direcciones IP o redes desde las que se originarán las pruebas                      | 10.10.1.0/24, 192.168.66.66, 10.20.15.123                                                                                                                                                                                                                                                                                                                                                                                    |
| Tipos de prueba permitidas o no permitidas                                          | Pruebas solo de aplicaciones web (app.secretcorp.org y app2.secretcorp.org). No se permiten ataques de ingeniería social. No se permiten ataques de inyección de SQL en el entorno d producción. La inyección de SQL solo se permite en los entornos de desarrollo y preparación en:<br> 1. app1-Dev.secretcorp.org<br> 2.- app1-stage.secretcorp.org<br> 3.- app2-dev.secretocorp.org<br> 4.- app2-stage.secretcorp.org<br> |
### 2.2.4 Lista de objetivos y activos dentro del alcance
El alcance es uno de los elementos más importantes de las tareas previas al compromiso con cualquier participación en una prueba de penetración. Ya que en ella se debe identificar y documentar cuidadosamente:
1. sistemas
2. aplicaciones
3. redes
Además de determinar los requisitos y calificaciones específicos necesarios para realizar la prueba.

Es posible ser contratado  para realizar una evaluación de aplicaciones modernas mediante diferentes interfaces de programación de aplicaciones conocidas normalmente como (API).

1. Archivos de proyecto del Protocolo Pimple de Acceso a Objetos (SOAP):
	1. Es un estándar que se basa en XML y esquemas relacionados. Las especificaciones basadas en XML se rigen por documentos de definición de esquema XML (XSD)
2. Swangger
	1. Es un marco moderno de documentación y desarrollo de API que ahora es la base de la especificación de OpenAPI. Estos documentos se utilizan en las API de transferencia de estado representacional (REST). REST es un estilo de arquitectura de software diseñado para guiar el desarrollo de la arquitectura de servicios web 
3. WSDL
	1. El Lenguaje de Descripción de Servicios Web (WSDL) es un lenguaje basado en XML que se utiliza para documentar la funcionalidad de un servicio web.
4. GraphQL
	1. Es un lenguaje de consulta para API. También es un tiempo de ejecución del lado del servidor para ejecutar consultas mediante un sistema de tipos que defina para sus datos.
Falta INFORMACIÓN
