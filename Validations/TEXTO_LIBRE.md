# NOMBRE/DESCRIPCIÓN
#input

 
#### Escenario \#6: `{campo}` válido.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** completo el campo  `{campo}` un valor alfanumérico  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `{campo}`

- - - -

#### Escenario \#7: `{campo}` sin completar.   
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** dejo el campo nombre sin completar  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono guardar  
**ENTONCES** el sistema previene la carga mostrando en el campo `{campo}` el mensaje “El campo es requerido”

- - - -

#### Escenario \#8: `{campo}` sólo espacios.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo el campo `{campo}` sólo con espacios  
**ENTONCES** el sistema muestra en el campo `{campo}` el mensaje “El campo es requerido”  

- - - -

#### Escenario \#9: `{campo}` con símbolos.   
  
**DADO** un administrador en la pantalla de  `{pantalla}`  
**Y** completo el campo  `{campo}` un valor que contiene símbolos y letras  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `{campo}`  

- - - -

#### Escenario \#10: `{campo}` solo símbolos.   
  
**DADO** un administrador en la pantalla de  `{pantalla}`  
**Y** completo el campo  `{campo}` un valor que contiene únicamente símbolos  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `{campo}`  

