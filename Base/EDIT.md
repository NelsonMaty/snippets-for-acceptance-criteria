# EDIT
#baseline


# Criterios de aceptación 
#### Escenario \#0: Errores en consola. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** abro la consola del navegador 
**CUANDO** realizo alguna acción sobre esta pantalla    
**ENTONCES** el sistema no escribe errores ni mensajes en la consola del navegador   

- - - -

#### Escenario \#1: Navegación.  
   
**DADO** un administrador en la vista de un `{recurso}`  
**CUANDO** hago click en el botón `✏️`  
**ENTONCES** la aplicación navega hacia la pantalla de editar `{recurso}`  
**Y** no veo errores ni mensajes en la consola del navegador  

- - - -

#### Escenario \#2: Función volver  
  
**DADO** un administrador en la pantalla de editar `{recurso}`  
**CUANDO** presiono el botón `Volver`   
**ENTONCES** la aplicación me dirige a la vista de un  `{recurso}` sin haber actualizado ningún dato  

- - - -

#### Escenario \#3: Función enlace directo  
  
**DADO** un administrador autenticado  
**CUANDO** ingreso a la URL  `{url}`  
**ENTONCES** veo el formulario para editar un  `{recurso}`  

- - - -
#### Escenario \#4: Campos bien nombrados.  
  
**DADO** un administrador en la pantalla de editar `{recurso}`  
**CUANDO** veo el formulario de edición  
**ENTONCES** los nombres de los campos son `{campos}`  

- - - -
#### Escenario \#5: Campos pre cargados.  
  
**DADO** un administrador
**CUANDO** accedo al formulario de edición  de un `{recurso}`  
**ENTONCES** los nombres de los campos `{campos}`  se muestran cargados con la información ya existente para el `{recurso}` seleccionado  

- - - -

#### Escenario \#6: Guardar y navegar.  
  
**DADO** un administrador en la pantalla de editar `{recurso}`  
**Y** modifico algunos de los campos presentes  
**CUANDO**  hago click en `Guardar`  
**ENTONCES** la aplicación muestra un modal de actualización exitosa y navega hacia la vista del `{recurso}`  con la información actualizada  

- - - -
  
#### Escenario \#7: Criterio de unicidad.  
  
**DADO** un administrador en la pantalla de editar `{recurso}`  
**Y** actualizo el campo `{campo_unico}` con un valor ya asociado a otro `{recurso}` cargado en el sistema  
**CUANDO**  hago click en `Guardar`  
**ENTONCES** veo un modal indicando que el registro ya existe en el sistema  
