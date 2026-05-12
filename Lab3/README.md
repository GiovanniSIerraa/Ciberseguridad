Laboratorio 3: Protocolos de Comunicación Seguros
Descripción de la Actividad

En este laboratorio se analizará la diferencia entre una comunicación insegura y una protegida mediante protocolos de seguridad. El objetivo principal es observar cómo la información enviada por una red puede ser interceptada cuando no existe cifrado y cómo herramientas como HTTPS, túneles SSH y VPN ayudan a proteger los datos.

Para el desarrollo de la actividad se utilizará Wireshark para capturar y analizar tráfico de red, además de servicios web configurados en un servidor Ubuntu.

¿Qué se realizará?

En una primera etapa se configurará un servidor web utilizando HTTP. Posteriormente, desde otra máquina se accederá a un formulario simple mientras se monitorea el tráfico con Wireshark. Esto permitirá visualizar información transmitida en texto plano, como nombres de usuario o contraseñas.

Luego, se implementarán mecanismos de seguridad para proteger la comunicación. Entre ellos, la configuración de HTTPS mediante certificados SSL y la creación de un túnel SSH para cifrar el tráfico entre cliente y servidor.

Finalmente, se volverá a analizar la red utilizando Wireshark con el objetivo de comprobar que la información ya no puede visualizarse de manera legible gracias al cifrado aplicado.

HERRAMIENTAS
Ubuntu Server (Servidor Web)
Kali Linux
Wireshark
Apache
SSH

¿Qué se observará?
Captura de tráfico HTTP sin cifrado utilizando Wireshark.
Visualización de información transmitida en texto plano.
Configuración de HTTPS en el servidor web.
Creación de un túnel SSH para proteger la comunicación.
Diferencia entre tráfico inseguro y tráfico cifrado.
Verificación de que la información ya no es legible tras aplicar seguridad.

La finalidad de este laboratorio es comprender la importancia de proteger las comunicaciones dentro de una red. A través del análisis de tráfico se podrá evidenciar cómo protocolos inseguros permiten interceptar información sensible.

Además, se busca entender cómo tecnologías como HTTPS, SSH y VPN permiten cifrar los datos transmitidos, aumentando la privacidad y reduciendo el riesgo de ataques o robo de información en entornos reales.
