# Cofiguración de Ansible


para comenzar primero instalamos y configuramos los 3 servicios siguientes:

<ul>
  <li>Apache</li>
  <li>Redis</li>
  <li>MySQL</li>
</ul>

<h2>Luego de haber hecho el paso anterior, procedemos con la instalación de los servidores web y de archivos.</h2>

## -Intalacion de Munin en los 3 servidores:

Para la instalacion de munin en en los 3 servidores utilizamos el siguiente comamdo 

ansible-playbook -i ../hosts inicial.yml

## -luego de lo anterior procederemos a instalar el servidor web en el server01

Utilizando el siguiente comando: 

ansible-playbook -i ../hosts webserver.yml

<h2>Ya habuiendo hecho lo anterior procederemos con la instalación del servidor Mysql.</h2>

## - Para este paso intalamos el servidor mysql en el server02

Utilizando el siguiente comando: 

ansible-playbook -i ../hosts sqlserver.yml

<h2>instalación de Redis.</h2>

## -Luego de completar el paso anterior procederemos a intalar Redis en el server03

Utilizando el siguiente comando: 

ansible-playbook -i ../hosts redis.yml

<h2>Instalacion de Moodle</h2>

## -Intalamos Moodle en el server02

Utilizamos el siguiente comando: 

ansible-playbook -i ../hosts moodle.yml










