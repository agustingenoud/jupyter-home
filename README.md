## Conectarse al server y bindiar puerto: ##

    ssh -L _(puerto_asignado)_:localhost:9999 _(usuario)_@ec2-3-23-88-218.us-east-2.compute.amazonaws.com

### Ejemplo: ###
    ssh -L _9999_:localhost:9999 _agustingenoud_@ec2-3-23-88-218.us-east-2.compute.amazonaws.com


Abrir docker-compose y cambiar:

    container_name: "(nombre_del_container_X)"

     ports:
      - "(puerto asignado):8888"
      
Correr `docker-compose up`