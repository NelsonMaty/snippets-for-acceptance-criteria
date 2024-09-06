# ACTIVO/INACTIVO
#input
- - - -

#### Escenario \#2: `{campo}` modificar estado a Inactivo.  
**DADO** un administrador en la pantalla `{pantalla}` de un proveedor  
**Y** modificado el valor del campo `{campo}` de Activo a Inactivo  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono `GUARDAR`  
**ENTONCES** el sistema muestra un modal de actualización exitosa y navega hacia la vista `Cuentas bancarias` de un proveedor con la información de `{campo}` actualizada  

- - - -

#### Escenario \#3: `{campo}` modificar estado a Activo.  
**DADO** un administrador en la pantalla `{pantalla}` de un proveedor  
**Y** modificado el valor del campo `{campo}` de Inactivo a Activo  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono `GUARDAR`  
**ENTONCES** el sistema muestra un modal de actualización exitosa y navega hacia la vista `Cuentas bancarias` de un proveedor con la información de `{campo}` actualizada  