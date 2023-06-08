# Abrir aplicaciones de desarrolladores No Identificados Archivo Dañado en macOS.


Ahora, en macOS también se verifican las aplicaciones iniciadas a través de la Terminal. Estos archivos obtienen el mismo escaneo de malware, verificación de firma y verificación de política de seguridad local. 
La diferencia en la primera ejecución, solo necesita aprobar explícitamente el software lanzado en paquetes, como un paquete de aplicaciones Mac estándar, no para ejecutables o bibliotecas independientes.

Con macOS Catalina en adelante, quizás de manera más significativa, Gatekeeper también verificará las aplicaciones y los archivos que no están en cuarentena en busca de problemas. No solo una o dos veces, sino cada vez que lo ejecuta. Cuando su Mac detecta un problema, bloquea el archivo y luego le envía una alerta.
Es la intención de Apple. 

Sin embargo, algunos desarrolladores pueden ver esto de manera diferente y encontrar los cambios en la terminal.

# Proceso:

-- 1º Camino
*En la terminal: sudo spctl --master-disable.
*Gatekeeper: https://n9.cl/or0sb

-- 2º Camino 
*En la Terminal: xattr -cr (ARRASTRARAMOS AQUÍ LA APP)

--3º Camino
*En la Terminal desactivar SIP(EN MODO RECUPERACIÓN): csrutil disable
*Para activar SIP: csrutil enable
