# LIST
#baseline


# Criterios de aceptación 

#### Escenario \#0: Errores en consola. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** abro la consola del navegador  
**CUANDO** realizo alguna acción sobre esta pantalla  
**ENTONCES** el sistema no escribe errores ni mensajes en la consola del navegador  

- - - -

#### Escenario \#1: Navegación  
**DADO** un administrador en la pantalla de ver `información general` de un `{recurso}`  
**CUANDO** hago clic en la opción `{subrecurso}`  
**ENTONCES** la aplicación navega hacia la pantalla de ver listado de `{subrecurso} de un {recurso}`  

- - - -

#### Escenario \#2: Función volver  
**DADO** un administrador en la pantalla `{subrecurso} de un {recurso}`  
**CUANDO** presiono el botón `Volver al listado`  
**ENTONCES** la aplicación me dirige a la pantalla del listado de `{recurso}`  

- - - -

#### Escenario \#3: Función enlace directo
**DADO** un administrador autenticado  
**CUANDO** ingreso a la URL `{url}`  
**ENTONCES** la aplicación navega hacia la pantalla de ver listado de  `{subrecurso} del {recurso}`  

- - - -

#### Escenario \#4: Columnas bien nombradas  
**DADO** un administrador en la pantalla `{subrecurso}` de un `{recurso}`  
**CUANDO** veo la tabla del listado  
**ENTONCES** los nombres de las columnas son `{campos}`  
**Y** la vista se titula `{subrecurso}`  

- - - -

#### Escenario \#5: Orden  
**DADO** un administrador en la pantalla `{subrecurso}` de un `{recurso}`  
**Y** existe mas de una `{subrecurso}`  
**CUANDO** veo la tabla del listado  
**ENTONCES** el listado se encuentra ordenado por la columna `{campo_orden}`  

- - - -

#### Escenario \#6: Paginación  
**DADO** un administrador en la pantalla `{subrecurso}` de un `{recurso}`  
**Y** existen más de 25 `{subrecurso}` registrados para dicho proveedor  
**CUANDO** veo la tabla del listado de `{subrecurso}`  
**ENTONCES** el listado consta sólo de 25 `{recurso}`  
**Y** hago scroll para ver el último registro de la tabla  
**ENTONCES** la tabla crece mostrando los siguientes 25 registros (si los hubiera)  


