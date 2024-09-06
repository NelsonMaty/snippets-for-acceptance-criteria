# CREATE
#baseline


# Criterios de aceptación 
#### Escenario \#0: Errores en consola.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** abro la consola del navegador  
**CUANDO** realizo alguna acción sobre esta pantalla  
**ENTONCES** el sistema no escribe errores ni mensajes en la consola del navegador  

- - - -

#### Escenario \#1: Navegación.  
   
**DADO** un administrador en el listado de `{recurso}`  
**CUANDO** hago click en el botón circular `+`  
**ENTONCES** la aplicación navega hacia la pantalla de agregar `{recurso}`  

- - - -

#### Escenario \#2: Función volver  
  
**DADO** un administrador en la pantalla de agregar `{recurso}`   
**CUANDO** presiono el botón `Volver`   
**ENTONCES** la aplicación me dirige a la pantalla del listado de `{listado}` sin haber creado un nuevo registro  

- - - -

#### Escenario \#3: Función enlace directo  
  
**DADO** un administrador autenticado  
**CUANDO** ingreso a la URL  `{url}`  
**ENTONCES** veo el formulario para crear un nuevo `{recurso}`  

- - - -
#### Escenario \#4: Campos bien nombrados.  
  
**DADO** un administrador en la pantalla de agregar `{recurso}`  
**CUANDO** veo el formulario de creación  
**ENTONCES** los nombres de los campos son `{campos}`  

- - - -

#### Escenario \#5: Guardar y navegar.  
  
**DADO** un administrador en la pantalla de agregar `{recurso}`  
**Y** completo el formulario con información válida  
**CUANDO**  hago click en `Guardar`  
**ENTONCES** la aplicación muestra un modal de creación exitosa  
**Y** navega hacia el listado de `{listado}` con el nuevo registro presente  

- - - -
  
#### Escenario \#6: Criterio de unicidad.  
  
**DADO** un administrador en la pantalla de crear  `{recurso}`  
**Y** completo el campo `{campo_unico}` con un valor ya asociado a otro `{recurso}` cargado en el sistema  
**CUANDO**  hago click en `Guardar`  
**ENTONCES** veo un modal indicando que el registro ya existe en el sistema  
