# Platzi-demo

En este proyecto, pretendo probar lo aprendido en el curso de DevOps dictado por [Platzi](https://platzi.com)
poniendo a prueba los ejercicios expuestos por el profesor Yamil Asusta @github/elbuo8 y haciendo pruebas de Integración Contínua usando [Docker](https://docker.com) y [CircleCi](https://circleci.com).

## ¿Qué es DevOps?

>DevOps (acrónimo inglés de development -desarrollo- y operations -operaciones-) es una práctica de ingeniería de software que tiene como objetivo unificar el desarrollo de software (Dev) y la operación del software (Ops). La principal característica del movimiento DevOps es defender enérgicamente la automatización y el monitoreo en todos los pasos de la construcción del software, desde la integración, las pruebas, la liberación hasta la implementación y la administración de la infraestructura. DevOps apunta a ciclos de desarrollo más cortos, mayor frecuencia de implementación, lanzamientos más confiables, en estrecha alineación con los objetivos comerciales.

Cita tomada de [Wikipedia](https://es.wikipedia.org/wiki/DevOps)

## ¿Qué son Integracion Continua y CircleCi?

>La integración continua (CI, por su sigla en inglés), es una manera que podemos probar código continuamente. Estos sistemas monitorean automáticamente nuevos Pull Request y otros eventos, y ejecutan automáticamente suites de prueba y otros chequeos automáticos, previamente configurados. 
>CircleCi, es un servicio para integración continua, y en resumen permite hacer build, test y despliegue de los lenguajes de programación más populares.

Cita tomada de [pybee.org](https://pybee.org/es/contribuir/como-ayudar/principiantes/que-es/ci/)

## ¿Qué es Docker?

>Docker es un proyecto de código abierto que automatiza el despliegue de aplicaciones dentro de contenedores de software, proporcionando una capa adicional de abstracción y automatización de virtualización de aplicaciones en múltiples sistemas operativos.2​ Docker utiliza características de aislamiento de recursos del kernel Linux, tales como cgroups y espacios de nombres (namespaces) para permitir que "contenedores" independientes se ejecuten dentro de una sola instancia de Linux, evitando la sobrecarga de iniciar y mantener máquinas virtuales.3​. 

Cita tomada de [Wikipedia](https://es.wikipedia.org/wiki/Docker_(software))

## Screenshots / Capturas de Pantalla


## Tech-framework used / Tecnologías Usadas
- Docker  17.05.0-ce 
	- Para [Linux](https://docs.docker.com/install/linux/docker-ce/debian/)
	- Para [Windows](https://docs.docker.com/docker-for-windows/) 
	- Para [Mac](https://docs.docker.com/docker-for-mac/)
- Node 8.11.4
	- express: ^4.16.4
	- mocha: ^5.2.0
	- supertest: ^3.3.0
	- now: 12.0.1

## Install / Instalación
#### OS X, Linux y Windows
*Abra un terminal y ejecute:*
```Shell
git clone http://github.com/pulidovpe/platzi-demo.git

cd platzi-demo

npm install

node server.js
```
Para ver la app en ejecución, luego de ejecutar los comandos anteriores, abrir el navegador en [localhost:3000](http://localhost:3000/)

Para ejecutar los test:
```Shell
mocha
```
Para construir el contenedor:
```Shell
docker build -t platzi .
```
Para ejecutar la app dentro del contenedor:
```Shell
docker run -d -p 3000:3000 platzi 
```
Para detener o matar el contenedor, debe averiguar su ID primero:
```Shell
docker ps 
```
Luego debe ejecutar el siguiente comando:
```Shell
docker kill  id_del_contenedor 
```

Para correr las pruebas de integración, debe tener una cuenta en CircleCi y asociarla con la de Github. Luego debe importar el proyecto generado.

## Tasks / Lista de Tareas
- [x] Inicialización de repositorio
- [x] Instalación de Docker
- [x] Desarrollo de aplicación
- [x] Desarrollo de las pruebas
- [x] Pruebas en local
- [x] Conexion con CircleCi
- [x] Pruebas de Integracion Continua
- [ ] Pruebas de despliegue usando Now.sh
- [ ] ...

## Contribute / Para contribuir
1. Has un [Fork](https://github.com/pulidovpe/platzi-demo/fork)
2. Crea tu propia rama (git checkout -b feature/fooBar)
3. Sube tus cambios (git commit -am 'Add some fooBar')
4. Actualiza tu rama (git push origin feature/fooBar)
5. Has un "Pull Request"

## Credits / Créditos
En este proyecto, me he guiado del curso de [Platzi](https://platzi.com/clases/1135-devops/) orientado a DevOps, de la documentacion oficial de [CircleCi](https://circleci.com/docs/2.0/) y la de [Docker](https://docs.docker.com/compose/).

## License / Licencia
Pulido V.P.E. – @github/pulidovpe – pulidovpe.dev@gmail.com
Distributed under the MIT license. See [LICENSE](LICENSE) for more information.
