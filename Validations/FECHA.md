# FECHA
#input

- - - -
    
#### Escenario \#10: `{nombre_campo}` válida.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** completo la `{nombre_campo}` con un formato de fecha válido `DD/MM/AAAA`  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `{nombre_campo}`  

- - - -
  
#### Escenario \#11: `{nombre_campo}` auto saneamiento.  
 
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** ingreso una letra, símbolo o número sin formato de fecha en el campo `{nombre_campo}`  
**Y** quito el foco del campo   
**ENTONCES** el sistema remueve los caracteres inválidos del campo `{nombre_campo}`  

- - - -
  
#### Escenario \#12: `{nombre_campo}` sin completar.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** dejo el campo `{nombre_campo}` sin completar  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono guardar  
**ENTONCES** el sistema previene la carga mostrando en el campo `{nombre_campo}` el mensaje “El campo es requerido”

- - - -

#### Escenario \#14: `{nombre_campo}` sólo espacios. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo el campo `{nombre_campo}` sólo con espacios  
**Y** quito el foco del campo  
**ENTONCES** el sistema muestra debajo del campo `{nombre_campo}` el mensaje de error  “El campo es requerido.“  