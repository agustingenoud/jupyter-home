Conectarse al server y bindiar puerto:

ssh -L (puerto_asignado):localhost:9999 (usuario)@ec2-3-23-88-218.us-east-2.compute.amazonaws.com

ejemplo:
    ssh -L 9999:localhost:9999 agustingenoud@ec2-3-23-88-218.us-east-2.compute.amazonaws.com


abrir docker-compose y cambiar:

    container_name: "(nombre_del_container_X)"
     ports:
      - "(puerto asignado):8888"