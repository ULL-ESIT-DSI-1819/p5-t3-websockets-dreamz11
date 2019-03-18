Simple App Chat
===================

Servidor de chat ejecutado en la maquina del iaas:

![](https://github.com/ULL-ESIT-DSI-1819/p5-t3-websockets-dreamz11/blob/master/Screenshot%20from%202019-03-18%2011-01-07.png)



Servidor de chat ejecutado en Heroku:

![](https://github.com/ULL-ESIT-DSI-1819/p5-t3-websockets-dreamz11/blob/master/Screenshot%20from%202019-03-18%2011-04-04.png)


![](https://github.com/ULL-ESIT-DSI-1819/p5-t3-websockets-dreamz11/blob/master/Screenshot%20from%202019-03-18%2011-04-17.png)


Para conseguir esto  por ejemplo ahora en la maquina del dsi se ha de completar los siguientes pasos:


Si no se tiene nada hecho se debe hacer un $heroku create para crear la aplicacion y un $git push heroku master - para
conseguir que se lanze la aplicacion y seguidamente con ps:scale web=1 se crea una instancia de nuestro programa

Primero se hace un login en heroku:

$ heroku login

Se clona el repositorio ya hecho anteriormente y funcionando

$ heroku git:clone -a blooming-gorge-41616
$ cd blooming-gorge-41616

y para comprobar si funciona se escala con el siguiente comando:

$heroku ps

y deberia salir que el servidor esta "up" .

Para hacer cambios se utiliza lo siguiente:

$ git add .
$ git commit -am "make it better"
$ git push heroku master

