# Comandos de Ubuntu

## Comandos basicos
| **Comando** | **Descripción**             | **Ejemplo**                        | **Explicación**                                                                                                                                |
| ----------- | --------------------------- | ---------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| `ls`        | Lista archivos y carpetas   | `ls -l`                            | Muestra el contenido del directorio actual. Con `-l` se obtiene una lista detallada con permisos, propietario, tamaño y fecha de modificación. |
| `cd`        | Cambia de directorio        | `cd /home`                         | Permite navegar entre carpetas. Por ejemplo, `cd /home` mueve al usuario al directorio `/home`.                                                |
| `cp`        | Copia archivos o carpetas   | `cp archivo.txt /tmp`              | Copia el archivo `archivo.txt` a la carpeta `/tmp`. También funciona con directorios si se usa `-r`.                                           |
| `mv`        | Mueve o renombra archivos   | `mv archivo.txt nuevo.txt`         | Sirve para mover archivos a otra ubicación o renombrarlos. Aquí, renombra `archivo.txt` a `nuevo.txt`.                                         |
| `rm`        | Elimina archivos o carpetas | `rm archivo.txt` o `rm -r carpeta` | Elimina archivos o directorios. `-r` es necesario para borrar carpetas con su contenido.                                                       |
| `chmod`     | Cambia permisos             | `chmod 755 script.sh`              | Modifica permisos de lectura, escritura y ejecución en archivos. El ejemplo da permisos de ejecución a todos.                                  |
| `chown`     | Cambia propietario          | `chown usuario:grupo archivo.txt`  | Cambia el dueño y el grupo de un archivo. Muy usado en administración de servidores.                                                           |
| `top`       | Procesos en tiempo real     | `top`                              | Muestra los procesos que se están ejecutando en el sistema en tiempo real, con uso de CPU y memoria.                                           |
| `ps`        | Lista procesos activos      | `ps aux`                           | Muestra todos los procesos en ejecución junto con su PID (identificador de proceso).                                                           |
| `kill`      | Finaliza procesos           | `kill 1234`                        | Termina un proceso usando su PID. Ejemplo: `kill 1234` mata el proceso con ID 1234.                                                            |

## Comandos intermedios 
| **Comando**       | **Descripción**                 | **Ejemplo**                                               | **Explicación**                                                                                     |
| ----------------- | ------------------------------- | --------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| `find`            | Buscar archivos por nombre      | `find /home -name "*.log"`                                | Busca archivos dentro de un directorio. Aquí, busca todos los `.log` en `/home`.                    |
| `grep`            | Buscar texto dentro de archivos | `grep 'ERROR' /var/log/syslog`                            | Busca líneas con la palabra `ERROR` dentro del archivo `/var/log/syslog`.                           |
| `apt / yum / dnf` | Gestión de paquetes             | `sudo apt install htop`                                   | Instala, actualiza o elimina paquetes. Ejemplo: `htop` se instala con apt.                          |
| `free`            | Uso de memoria                  | `free -h`                                                 | Muestra la memoria RAM y el uso de swap en el sistema. `-h` lo presenta en formato legible (MB/GB). |
| `df`              | Uso de disco                    | `df -h`                                                   | Muestra el espacio usado y disponible en las particiones del disco.                                 |
| `du`              | Tamaño de carpetas              | `du -sh /var/log`                                         | Calcula el tamaño total de una carpeta. En este caso, el directorio `/var/log`.                     |
| `htop`            | Monitor interactivo             | `htop`                                                    | Similar a `top`, pero con interfaz más amigable y permite interactuar con los procesos.             |
| `adduser`         | Crear usuario                   | `sudo adduser devops`                                     | Crea un nuevo usuario en el sistema. Aquí, se crea el usuario `devops`.                             |
| `usermod`         | Modificar usuario / grupos      | `sudo usermod -aG docker devops`                          | Agrega al usuario `devops` al grupo `docker`.                                                       |
| `groups`          | Ver grupos de un usuario        | `groups devops`                                           | Muestra a qué grupos pertenece un usuario.                                                          |
| `ip`              | Interfaces de red               | `ip a`                                                    | Lista las interfaces de red, direcciones IP y estado de cada una.                                   |
| `ping`            | Probar conectividad             | `ping google.com`                                         | Envía paquetes a un host para comprobar si responde. Muy usado para probar conexión a internet.     |
| `netstat`         | Ver puertos en uso              | `netstat -tulnp`                                          | Lista las conexiones de red activas y qué procesos están usando cada puerto.                        |
| `tar`             | Comprimir/Descomprimir          | `tar -czvf backup.tar.gz /home/usuario`                   | Comprime una carpeta en un archivo `.tar.gz`.                                                       |
| `zip / unzip`     | Comprimir/Descomprimir          | `zip -r proyecto.zip proyecto/` <br> `unzip proyecto.zip` | Crea un archivo `.zip` o lo descomprime.                                                            |

## Comandos avazados
| **Comando** | **Descripción**                                | **Ejemplo**                                  | **Explicación**                                                                                                                                                           |
| ----------- | ---------------------------------------------- | -------------------------------------------- | -------------------------------------------------------------------------------------- | 
| `ps aux`    | Buscar procesos por nombre                     | `grep nginx`                                 | Filtra procesos que coincidan con un nombre. Aquí busca si `nginx` está corriendo. | 
| `pkill`     | Finalizar procesos por nombre                  | `pkill -9 python`                            | Mata todos los procesos que tengan el nombre `python`.                                 |              
| `alias`     | Crear alias de comandos                        | `alias ll='ls -la'`                          | Permite crear atajos para comandos largos. Aquí, `ll` equivale a `ls -la`.             |              
| `history`   | Ver historial de comandos                      | `history`                                    | Muestra la lista de comandos ejecutados por el usuario.                                |              
| `!<cmd>`    | Ejecutar último comando que inicia con `<cmd>` | `!ls`                                        | Ejecuta el último comando que comenzaba con `ls`.                                      |              
| `crontab`   | Programar tareas automáticas                   | `crontab -e`                                 | Abre el archivo de configuración de tareas programadas. Útil para automatizar scripts. |              
| `scp`       | Transferir archivos                            | `scp archivo.txt usuario@192.168.1.10:/home` | Copia archivos de forma segura entre equipos usando SSH.                               |              
| `ssh`       | Conexión remota a servidor                     | `ssh usuario@ip_servidor`                    | Permite acceder de forma remota a otro sistema mediante el protocolo SSH.              |              

## Imagenes 

#### Para poder subir imagenes es con un comando en el README simple 
![Comando para imagenes](ejemplo.png)
#### Con este comando podremos subir imagenes a nuestro README 
#### por ejemplo el logo del SENA
![Logo del SENA](imagen.png)

## Base de datos
#### diseno
![Diseño base de datos](basededatosTechCol.png)

### Inserts de las tablas:

#### INSERT INTO roles (roleId, roleName) VALUES (1, 'Admin');
#### INSERT INTO roles (roleId, roleName) VALUES (2, 'Cliente');

#### INSERT INTO customers (customerId, customerName, customerLastName, customerEmail, customerPassword, customerPhoneNumber, roleId) VALUES (1, 'Juan', 'Pérez', 'juanperez@example.com', 'pass123', '3001234567', 2);

#### INSERT INTO customers (customerId, customerName, customerLastName, customerEmail, customerPassword, customerPhoneNumber, roleId) VALUES (2, 'Ana', 'Gómez', 'anagomez@example.com', 'pass456', '3017654321', 2);

#### INSERT INTO adresses (adressId, street, city, state, postalCode, country, customerId) VALUES (1, 'Calle 123', 'Bogotá', 'Cundinamarca', '110111', 'Colombia', 1);

#### INSERT INTO adresses (adressId, street, city, state, postalCode, country, customerId) VALUES (2, 'Carrera 45', 'Medellín', 'Antioquia', '050020', 'Colombia', 2);

#### INSERT INTO products (productId, productName, productDescription, unitPrice, productStock) VALUES (1, 'Mouse Gamer', 'Mouse óptico RGB', 80.50, 100);

#### INSERT INTO products (productId, productName, productDescription, unitPrice, productStock) VALUES (2, 'Teclado Mecánico', 'Teclado retroiluminado', 150.00, 50);

#### INSERT INTO carts (cartId, cartPrice, createdAt, customerId) VALUES (1, 230.50, '2025-09-12 10:30:00', 1);

#### INSERT INTO carts (cartId, cartPrice, createdAt, customerId) VALUES (2, 150.00, '2025-09-12 11:00:00', 2);

#### INSERT INTO cart_details (cartDetailId, quantity, unitPrice, cartId, productId) VALUES (1, 2, 80.50, 1, 1);

#### INSERT INTO cart_details (cartDetailId, quantity, unitPrice, cartId, productId) VALUES (2, 1, 150.00, 2, 2);

#### INSERT INTO orders (orderId, orderPrice, orderDate, customerId, cartId) VALUES (1, 161.00, '2025-09-12 12:00:00', 1, 1);

#### INSERT INTO orders (orderId, orderPrice, orderDate, customerId, cartId) VALUES (2, 150.00, '2025-09-12 12:15:00', 2, 2);

#### INSERT INTO order_details (orderDetailId, quantity, unitPrice, orderId, productId) VALUES (1, 2, 80.50, 1, 1);

#### INSERT INTO order_details (orderDetailId, quantity, unitPrice, orderId, productId) VALUES (2, 1, 150.00, 2, 2);

#### INSERT INTO shipments (shipmentId, shipmentStatus, trackingNumber, shipmentDate, orderId) VALUES (1, 'SHIPPED', 'TRK12345', '2025-09-13 09:00:00', 1);

#### INSERT INTO shipments (shipmentId, shipmentStatus, trackingNumber, shipmentDate, orderId) VALUES (2, 'PENDING', 'TRK67890', '2025-09-13 09:15:00', 2);

#### INSERT INTO payments (paymentId, paymentMethod, paymentStatus, transactionId, amountPaid, paymentDate, orderId) VALUES (1, 'CREDIT_CARD', 'APPROVED', 'TXN1001', 161.00, '2025-09-12 12:30:00', 1);

#### INSERT INTO payments (paymentId, paymentMethod, paymentStatus, transactionId, amountPaid, paymentDate, orderId) VALUES (2, 'PAYPAL', 'PENDING', 'TXN1002', 150.00, '2025-09-12 12:45:00', 2);

#### INSERT INTO logs (logId, action, timestamp, customerId) VALUES (1, 'Inicio de sesión', '2025-09-12 09:00:00', 1);

#### INSERT INTO logs (logId, action, timestamp, customerId) VALUES (2, 'Creación de pedido', '2025-09-12 12:00:00', 2);