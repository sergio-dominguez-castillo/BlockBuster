# README

Requerimientos
1. Set-up inicial del proyecto, el proyecto viene con algunos errores que deben ser
corregidos y cargar datos ficticios.
(2 Puntos)
Recuerda el uso de la gema faker.
2. Al editar una película puedo asignarle un cliente.
(2 Puntos)
3. En el index de clientes mostrar si el cliente tiene una película arrendada.
(2 Puntos)
4. Modificar diseño de la aplicación, no puede ser igual al entregado.
(2 Puntos)
Toda aplicación debe ser atractiva a la vista.
5. Hacer deploy a heroku.
(2 puntos)

Nota: mis tarjetas de debito no me funcionaron en heroku, puedo acceder a servicios de streaming pero imposible a heroku, me rechazo todas mis tarjetas

explico las opciones que disponemos par deloyment en heroku

tenemos dos opciones
1 consola

1. realizamos login a heroku, con el comando heroku login
2. creamos la aplicacion, con el comando heroku create
3. subimos la aplicacion
	a. git init
	b. heroku git:remote -a nombre de tu proyecto creado en Heroku.
	c. git add .
	d. git commit -am "Feat: Primer commit to push to heroku"
	e. git push heroku main
	
cualquier mejora o actualizacion de la app
Dado que nuestra aplicación está enlazada a git debemos subir estos cambios,
repitiendo el proceso de:
	a. git add .
	b. git commit -m ”Describe el cambio realizado”
	c. git push heroku main

2 heroku + github

1. subir a github
	a. git add .
	b. git commit -m ”Describe el cambio realizado”
	c. git push origin main (o la rama)   
	
2. pull request
	a. con integracion continua ci/cd
	luego merge pull request
	confirm merge  -> lleva los cambios a main (github)

3. Nota: nos traemos la app a local con toda la integracion continua (ci/cd) del paso anterior
	git checkout main
	luego git pull origin main

4. ahora voy a heroku a crear la app
	a. 	le asigo el nombre de la app
	b. 	luego selecciono el metodo de deployment GitHub 	y lo conecto con la app que esta en github
	c. 	luego en automatic deploy, selecciono wait for CI to pass defore deploy (esperar a que termine la integracion continua en github
	d.	o voy a manual deploy, selecciono el branch  to deploy (main) y doy clic en deply branch 




