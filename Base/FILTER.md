# FILTER
#baseline


# Criterios de aceptación 

#### Escenario \#0: Errores en consola. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** abro la consola del navegador  
**CUANDO** realizo alguna operación de filtro sobre esta pantalla  
**ENTONCES** el sistema no escribe errores ni mensajes en la consola del navegador  

- - - -
#### Escenario \#1: Campos bien nombrados.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** veo el formulario de búsqueda  
**ENTONCES** los nombres de los campos son `{campos}`  

- - - -
#### Escenario \#2: Aplicar filtros
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo los campos  
**Y** hago click en el botón Aplicar Filtros  
**ENTONCES** se actualiza el listado de `{recursos}`  
**Y** el botón no es clickable durante la búsqueda  

- - - -
#### Escenario \#3: Limpiar filtros
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo los campos  
**Y** hago click en el botón Limpiar Filtros  
**ENTONCES** se actualiza el listado de `{recursos}`  
**Y** los campos del formulario de búsqueda se vacían  
**Y** el botón no es clickable durante la búsqueda  

- - - -
#### Escenario \#4: Orden
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** realizo una búsqueda  
**ENTONCES** los resultados se muestran ordenados por el campo `{campo_orden}`  

- - - -
#### Escenario \#5: Búsqueda por `{campo}`  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo el campo `{campo}`  
**Y** hago click en el botón Aplicar Filtros  
**ENTONCES** el listado sólo muestra `{recursos}` cuyos `{campo}` contenga la palabra buscada de forma parcial o total.  


- - - -
#### Escenario \#8: Búsqueda multi criterios
  
**DADO** un administrador en la pantalla de `{pantalla}`   
**CUANDO** completo más de un campo de búsqueda   
**ENTONCES** los resultados son acordes a los múltiples criterios de búsqueda que ingresé  