# DELETE
#baseline

#### Escenario \#0: Errores en consola. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** abro la consola del navegador  
**CUANDO** realizo alguna acción sobre esta pantalla  
**ENTONCES** el sistema no escribe errores ni mensajes en la consola del navegador  

- - - -
#### Escenario \#1: Modal de confirmación.  
  
**DADO** un administrador en la pantalla de ver `{recursos}`    
**Y** existe al menos un registro creado  
**CUANDO** hago click en el símbolo 🗑 de un registro  
**ENTONCES** veo un modal de confirmación mencionando el `número de factura` asociado al registro que deseo eliminar  

- - - -
#### Escenario \#2: Cancelar modal.  
  
**DADO** un administrador en la pantalla de ver `{recursos}`   
**Y** hago click en el símbolo 🗑 de un registro  
**CUANDO** hago click en el botón Cancelar del modal  
**ENTONCES** el modal se cierra  
**Y** ningún registro se elimina en el listado

- - - -
#### Escenario \#3: Aceptar modal.  
  
**DADO** un administrador en la pantalla de ver `{recursos}`    
**Y** hago click en el símbolo 🗑 de un registro  
**CUANDO** hago click en el botón Aceptar del modal  
**ENTONCES** el modal se cierra  
**Y** veo momentáneamente un modal de operación exitosa  
**Y** el registro no está presente en el listado de `{recursos}`
