---

description: Initial description.

author: "@Luigi"
---

- Preguntas para Dani
	- Usas yarn o npm?
	- TODO mirar gulp para hacer build de JS y css
	- Vale la pena usar themekit para desarrollo en local (hacen falta claves para themekit)
	- ~~Hay que lanzar `theme watch`? me pide un config.yml que no hay~~
	- Me pueden confirmar que `dztesting.myshopify.com` es QA y que `ringrover.myshopify.com` es PROD?
	- No puedo descargar el theme de producción (revisar porque quizás hago algo mal)
	- Uno de los tiquets se refiere a https://ringrover.myshopify.com/admin/orders/4465998757923 (abajo del todo). Podemos nosotros programar esta web (el admin)? Quizás esto sea solo BackEnd related?
	- En el otro ticket, no tengo claro lo que hay que hacer
- Aclarar con Dani
	- Como crear una branch para development a partir de la branch master que hay
	- En QA (https://dztesting.myshopify.com/admin/themes) puedo eliminar themes que hay creados?
- Demo today
	- what is OTA?
	- spoton-api-qa.herokuapp.com/admin
- TODO: sincronizar el repo con producción. (se comenta en el video en el minuto 20')
	- Descargar el código de producción y comprarar con Meld para ver el alcance.
- TODO: mirar si tengo acceso a Pagefly
- TODO: aprender (con Dani) a hacer deploy a production
- TODO: mirar si tengo accesos a pagefly
- Saber las url de prod y qa
-
- Como puedo enviar lo que tengo en QA a prod, es peligroso verdad?
	- Puedo hacer cambios en el backoffice de producción (para probar) sin que se publique? Imagino que hay que apretar "Save" para guardar les cambio, verdad? (he modificado tamaño de imágenes por accidente, pero no he apretado "Save")
- theme deploy sobre el theme de production.
- si veo cambios directos hay que aplicar en scss
-
- REUNIÓN CON MATEO
	- Preguntar si Dani u otra persona hará las CR
	- ANDY hará los diseños
-
- landing ara SSR
- Homepage
- loged in RN
-
-
- GULP adventure
	- npm install -g gulp-cli
	- gulp watch gives error and need to put overrides at package.json
	- ```
	  "overrides": {"graceful-fs": "^4.2.10"}
	  ```
	- Looks like I need to  downgrade node to v14
		- nvm install 14.15.0
		- nvm use 14.15.0
		- npm install -g gulp-cli (again!)
		- gulp watch error again
			- npm rebuild node-sass
			-
		-
	-
- theme watch --allow-live
-
- theme deploy sobre el theme de production.
- si veo cambios directos hay que aplicar en scss
-
- He puesto los archivos descargados en la carpeta (y en una nueva branch)
- He puesto a correr gulp watch
- theme watch --allow-live
-
- Pasos a seguir:
	- Comparar con meld (o mediante git en VScode)
	- Hay que hacer algun build?
	- Como usar config.yml?
		- ```
		  development:
		  password: shptka_25c53470a95aa4526616e6f96d708bb7
		  theme_id: "127735234725"
		  store: dztesting.myshopify.com
		  ```
		- Este es el del branch, usa el id del theme activo de QA
		-
	- TODO commit en branch merge-production
	- TODO merge merge-production a master después de testear
	- TODO crear de nuevo DOG-1329 desde nuevo master y aplicar patch con los cambios de la card.
	- TODO mover card a QA merge de DOG-1329 a master
	- TODO deploy de master a Copia de Prod
		- Simplemente: theme build 121991594019 (este id es copia de prod)
		- Para prod seria theme build 120611340323 ???
		-
	- volver a descargar theme de prod y compararar con meld antes de gulp watch.
	- sections templates assets(theme.js theme.css) layouts
-
- DOG-1376
- DOG-1377 with static images.
- DOG-1378 sprint que viene.
-
- SPOTON deploy to QA
	- Command list https://shopify.dev/themes/tools/theme-kit/command-reference
		- Basically
			- theme deploy --env=production
			- theme deploy (currently fails)
			- theme download ???
		-
		-
		-
		- 1 descargar imagenes y subirlas
		- crear los menus (con 1 item)
		- vuelvo a bajar el theme de prod
		- lo añado a qa (pero ahora debería enseñar las imágenes)
		- descargar el theme de production en un branch de git
		- Vuelvo a poner los cambios antes de gulp
		- ejecuto gulp y theme deploy o poner en zip y crear un theme nuevo
		- descargo el de qa y el de prod y hago diff para ver que hay pocos cambios
		- creas nuevo theme con el .zip de qa y publicas.
		-
		-
		-
		-