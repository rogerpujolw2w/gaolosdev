# Gaolos

GaolosDev es un proyecto realizado en Angular 8.0.4 (https://github.com/angular/angular-cli), y es un ERP, copia de un actual proyecto generado en Core Net.

El proyecto se encuentra en GitHub pero está en modo privado, ya que para hacer las primeras pruebas se incrustó en el codigo información personal real.

Este proyecto, tal y como está diseñado en Core Net, es perfecto para aplicar el Angular por los siguientes motivos:

- Se usa el modelo MVC, así que es perfecto para migrar a Angular
- Toda la lógica de negocio se basa en servicios Rest - Api
 

No hay versión funcional por falta de tiempo. La idea es usar este proyecto para el Mean Stack 3.


Las APIs que gestionan toda la aplicación se encuentran en:

-  https://xxx.gaolos.com/ (Publicado en servidores privados)

La idea inicial para hacer este proyecto es que tuviese los siguientes módulos:

## Módulo Servicios

En el módulo Servicios tenemos un CRUD en el cual podemos crear nuevos servicios, listarlos y ver el detalle del mismo.
Los componentes utilizados serían:

- **SERVICIO**: formulario de crear nuevo servicio, editar y eliminar
- **SERVICIOS**: vista del listado de servicios. Desde aquí podemos ir a SERVICIO, para editar y eliminar.

## Módulo MiEmpresa

El módulo de Mi Empresas tenemos otro CRUD que nos permite visualizar los usuarios.

- **NUEVOUSUARIO**: formulario para crear nuevos usuarios dentro de mi empresa
- **USUARIO**: formulario para modificar el usuario
- **USUARIOS**: vista del listado de usuarios. Desde aquí podemos ir a la ficha del Usuario para ver/editar , y también podremos eliminar.

## Módulo Commons

- **HOME**: Pantalla de login
- **INICIO**: Pantalla de bienvenida una vez logado (Ruta protegida)
- **NAVBAR**: Barra de navegación
- **MENULATERAL**: Menú lateral con los módulos disponibles para el usuario
- **BARRASUPERIOR**: Opciones del usuario y acceso a sus datos
- **BARRAINFERIOR**: Información del módulo en el que estamos
- **NOTFOUND**: 404 error

No usamos:
- **FOOTER**: Pie de la web, ya que nos es una herramienta comercial


## SHARED

En la carpeta 'shared' encontramos los servicios utilizados, las clases y el auth-guard

- **MODELS**: Donde guardamos las clases básicas
- **GUARDS**: Bloquea el acceso a 'nueva-oferta' si no hemos hecho login
- **SERVICIOS**: Api.Service gestiona la comunicación con las Api-Rest y Auth.Service 

 ## API

https://xxx.gaolos.com/

## DEPENDENCIAS UTILIZADAS

- Bootstrap
- JQuery
- **NGX Spinner** (https://napster2210.github.io/ngx-spinner/)
- **Moment.js** (https://www.npmjs.com/package/moment)

## RETO A SUPERAR

- Aplicar todas las funcionalidades que tenemos el Ajax y JQuery en Angular
- Mejorar la experiencia del usuario mediante Angular


## FUTURIBLES

Usar librerías reactivas o Sockets para poder actualizar la información que visualiza el usuario en tiempo real, cuando es modificada por otro usuario.


Otras mejoras a realizar son:

- Migrar los servicios Rest en Core Net a Node
- Migrar las bases de datos a MongoDB


