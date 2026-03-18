SEMANA 2 - Guía de Trabajo Práctico - Desafío de Arquitectura - De On-Premise a la Nube 

¡Hola a todos! Durante esta segunda semana de clases nos enfocaremos en entender cómo se estructuran las redes empresariales tradicionales (On-Premise) y cómo se comparan con las soluciones en la nube (Cloud Computing). Para poner en práctica estos conceptos, resolverán el siguiente caso de estudio. Lean con atención cada paso y tómense un momento para pensar en las "Pausas de Reflexión" antes de escribir sus respuestas.

--------------------------------------------------------------------------------

El Caso de Estudio: La expansión de "Distribuidora Rápida" "Distribuidora Rápida" es una empresa de logística que maneja todo su inventario y rutas desde sus oficinas centrales. Actualmente, toda su infraestructura tecnológica es On-Premise. Tienen una sala de servidores (Data Center local) que incluye: 

● 3 Servidores físicos (uno para base de datos, uno para la aplicación de inventario y uno para respaldos). 

● 1 Firewall físico conectado al router del proveedor de internet. 

● Equipos de aire acondicionado dedicados para mantener los servidores fríos. 

● Un técnico contratado a tiempo completo solo para el mantenimiento de los fierros (hardware). La empresa planea abrir 5 nuevas sucursales en diferentes ciudades el próximo mes y necesita que todas accedan al sistema de inventario al mismo tiempo. El técnico les ha advertido que los servidores actuales no soportarán tanto tráfico y que comprar nuevos servidores tomará al menos 2 meses entre envío e instalación. 

-------------------------------------------------------------------------------- 

PASO 1: Análisis de la Arquitectura On-Premise Actual Basándote en la descripción del caso, identifica los principales desafíos de la red tradicional que tiene la empresa. 1. Haz una lista de los componentes físicos que "Distribuidora Rápida" tiene que mantener y pagar actualmente, los usen a su máxima capacidad o no. 2. Explica brevemente cuál es el mayor "cuello de botella" tecnológico que enfrentan para lograr su expansión de forma rápida. 

💡 Pausa de Reflexión: Imagina que mañana ocurre un corte de luz masivo en la cuadra de la oficina central de la empresa o el aire acondicionado se descompone durante un fin de semana. 

¿Qué pasaría con las 5 nuevas sucursales que dependen de esa sala de servidores?

¿De quién es la responsabilidad de arreglarlo? 

PASO 2: Diseñando el salto al Cloud Computing El gerente de la empresa te contrata como consultor en arquitectura TI y te pide una solución rápida. Tú le sugieres migrar a un modelo de Cloud Computing.
1. Describe cómo se transformarían los 3 servidores físicos y el firewall físico si los pasaran a la nube (por ejemplo, a servicios como AWS, Azure o Google Cloud). 
2.  Explica cómo la nube solucionaría el problema de los "2 meses de espera" para tener los nuevos servidores listos para la expansión. 💡 Pausa de Reflexión: Al mover todo a la nube, la empresa ya no necesitará pagar la cuenta de luz del aire acondicionado ni el espacio físico de la sala de servidores. Sin embargo, empezarán a pagar una factura mensual al proveedor de la nube. 

	¿Crees que están ahorrando dinero o simplemente cambiando el tipo de gasto? 
	
PASO 3: Análisis Comparativo Final Para convencer al gerente de "Distribuidora Rápida" con datos claros, elabora un Cuadro Comparativo entre mantener su arquitectura On-Premise actual o migrar al Cloud Computing.

![[Pasted image 20260318144754.png]]

💡 Pausa de Reflexión: Mira la última fila de tu tabla ("Control físico de los datos"). Si bien la nube ofrece muchas ventajas para expandirse rápido, ¿en qué tipo de industrias (por ejemplo, bancos, hospitales, fuerzas armadas) crees que una empresa preferiría quedarse con una arquitectura On-Premise a pesar de ser más lenta de escalar? ¿Por qué? 

-------------------------------------------------------------------------------- 

Entregable: Redacta tus respuestas y tu cuadro comparativo en un documento limpio. ¡Prepárense para debatir sus conclusiones de la "Pausa de Reflexión" en nuestra próxima clase!

| **Criterio a evaluar**          | **Arquitectura Tradicional (On-Premise)**                | **Informática en la Nube (Cloud Computing)**                         |
| ------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------- |
| **Tiempo de implementación**    | Lento (semanas o meses para compra y configuración)      | Inmediato (minutos, a través de una consola)                         |
| **Mantenimiento del Hardware**  | Responsabilidad total de la empresa (técnico interno)    | Responsabilidad del proveedor de nube (transparente para el usuario) |
| **Escalabilidad**               | Limitada y difícil; requiere comprar más equipos físicos | Alta y rápida; crece o disminuye según la demanda automáticamente    |
| **Control físico de los datos** | Total; el servidor está físicamente en la oficina        | Delegado; los datos residen en centros de datos del proveedor        |
