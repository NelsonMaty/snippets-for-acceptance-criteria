# VIEW
#baseline

# Criterios de aceptación 

#### Escenario \#0: Errores en consola. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** abro la consola del navegador  
**CUANDO** realizo alguna acción sobre esta pantalla  
**ENTONCES** el sistema no escribe errores ni mensajes en la consola del navegador  

- - - -

#### Escenario \#1: Navegación.  
   
**DADO** un administrador en el listado de `{recursos}`  
**CUANDO** hago click en el botón `👁`  
**ENTONCES** la aplicación navega hacia la pantalla de ver  `{recurso}` con la información del proveedor seleccionado  

- - - -

#### Escenario \#2: Función volver  
  
**DADO** un administrador en la pantalla de agregar `{recurso}`  
**CUANDO** presiono el botón `Volver al listado`  
**ENTONCES** la aplicación me dirige a la pantalla del listado de `{recursos}`  

- - - -

#### Escenario \#3: Función enlace directo  
  
**DADO** un administrador autenticado  
**CUANDO** ingreso a la URL `{url}`  
**ENTONCES** la aplicación navega hacia la pantalla de ver `{recurso}`  

- - - -
#### Escenario \#4: Campos bien nombrados.  
  
**DADO** un administrador en la pantalla de ver `{recurso}`  
**CUANDO** veo los campos mostrados  
**ENTONCES** los nombres de los campos son `{campos}`  
**Y** la vista se titula `Información general`  
**Y** los valores son correctos  

- - - -
  
#### Escenario \#5: Información incompleta.  
  
**DADO** un `{recurso}`  que no tiene  `{campo_incompleto}` asociado  
**CUANDO** solicito la información de dicho `{recurso}`  
**ENTONCES** veo dos guiones "--" en lugar del valor del `{campo_incompleto}`  

