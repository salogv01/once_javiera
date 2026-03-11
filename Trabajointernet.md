# El Internet



## Origen del Internet



En el video se explica que el internet nació a partir de ARPANET (Advanced Research Projects Agency Network), la primera red creada en 1969 por el Departamento de Defensa de EE.UU.



Fue diseñada para interconectar computadores que se encontraban en lugares inaccesibles y permitir la comunicación entre ellos.



## Cómo viajan los datos



Los datos se envían en forma de paquetes, que viajan a través de routers (dispositivos de red) por distintas rutas geográficas hasta llegar a su destino.



Los routers se comunican mediante protocolos, entre los principales están:



IP (Internet Protocol)  

Asigna una dirección única a cada dispositivo conectado a la red.  

- IPv4: 32 bits (aproximadamente 4,000 millones de direcciones).  

- IPv6: 128 bits (diseñado para cubrir la demanda futura).



TCP (Transmission Control Protocol)  

Se encarga de identificar servicios específicos mediante números de puertos y garantizar una entrega confiable de los datos.



## DNS: nombres en lugar de números



Sería complicado escribir una dirección IP cada vez que queremos acceder a un sitio web.



Para esto existe el Domain Name System (DNS), que funciona como una guía telefónica y traduce los nombres de dominio como example.com en direcciones IP.



## DHCP: asignación automática de IP



Los dispositivos obtienen su dirección IP automáticamente gracias al protocolo DHCP (Dynamic Host Configuration Protocol), que asigna la configuración de red necesaria.



## HTTP y las páginas web



Para solicitar y recibir páginas web se utiliza el protocolo HTTP (HyperText Transfer Protocol).



Este utiliza una URL, que está compuesta por:



- Esquema: https  

- Nombre de host: www  

- Dominio: example.com  

- Ruta: archivo o directorio específico  



Las solicitudes utilizan verbos como:



- GET: solicitar datos  



Los servidores responden con códigos que indican el resultado de la solicitud:



- 200 OK: todo correcto  

- 301 Moved Permanently: redirección  

- 404 Not Found: archivo no encontrado  



## Herramientas útiles



curl: programa que permite ver en la terminal los encabezados de respuesta HTTP.  



inspect: comando del navegador que abre las herramientas de desarrollador, permitiendo ver el tráfico de red y el código de los sitios web en tiempo real.





- Salomé González Valencia  

- Tomás Martínez Tangarife  

- Juan Manuel Muñoz Castro  