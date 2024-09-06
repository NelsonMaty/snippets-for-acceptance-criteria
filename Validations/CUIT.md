# CUIT
#input

- - - -
    
#### Escenario \#10: `CUIT` válido.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** completo el `CUIT` con un valor numérico entero positivo de largo 11  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `CUIT`

- - - -
  
#### Escenario \#11: `CUIT` alfanumérico.  
 
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** ingreso una letra en el campo `CUIT`  
**ENTONCES** el sistema muestra debajo del campo `CUIT` el mensaje de error “El campo debe contener solo caracteres numéricos.“   

- - - -
  
#### Escenario \#12: `CUIT` sin completar.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**Y** dejo el campo `CUIT` sin completar  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono guardar  
**ENTONCES** el sistema previene la carga mostrando en el campo `CUIT` el mensaje “El campo es requerido”

- - - -
  
#### Escenario \#13: `CUIT` con símbolos.  
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** ingreso un símbolo  
**ENTONCES** el sistema muestra debajo del campo `CUIT` el mensaje de error  “El campo debe contener solo caracteres numéricos.“  

- - - -

#### Escenario \#14: `CUIT` sólo espacios. 
  
**DADO** un administrador en la pantalla de `{pantalla}`  
**CUANDO** completo el campo `CUIT` sólo con espacios  
**ENTONCES** el sistema muestra debajo del campo `CUIT` el mensaje de error  “El campo debe contener solo caracteres numéricos.“  