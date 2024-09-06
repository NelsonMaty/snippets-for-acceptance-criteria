# EMAIL
#input

- - - -
  
#### Escenario \#15: `Correo` formato válido.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** completo el campo Correo electrónico con un valor que respete el formato “caracteres alfanuméricos y/o símbolos” + “@“ + “carácteres alfanuméricos y/o símbolos” + “.” + “carácteres alfanuméricos y/o símbolos”  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `Correo electrónico`  

- - - -

#### Escenario \#16: `Correo electrónico` sin completar.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** completo los demás campos del formulario con valores válidos  
**CUANDO** presiono guardar    
**ENTONCES** el sistema guarda los datos correctamente sin mensajes de error  

- - - -

#### Escenario \#17: `Correo electrónico` sólo espacios. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo el campo nombre sólo con espacios  
**ENTONCES** el sistema muestra en el campo `Correo electrónico` el mensaje “El campo debe ser un correo electrónico válido.”  
