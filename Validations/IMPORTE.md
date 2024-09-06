# IMPORTE
#input


#### Escenario \#10: `Importe` válido.  
**DADO** un administrador en la pantalla `{pantalla}`  
**Y** completo el campo `Importe` con un valor numérico entero positivo  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `Importe`  
**Y** el importe lo veo formateado con puntos donde corresponden (miles, millones, etc)

- - - -

#### Escenario \#11: `Importe` alfanumérico.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** ingreso una letra en el campo `Importe`  
**ENTONCES** el sistema muestra debajo del campo `Importe` el mensaje de error “No se respeta el formato moneda.“  

- - - -

#### Escenario \#14: `Importe` sin completar.  
**DADO** un administrador en la pantalla `{pantalla}`  
**Y** dejo el campo `Importe` sin completar  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono `GUARDAR`  
**ENTONCES** el sistema previene la carga mostrando en el campo `Importe` el mensaje “El campo es requerido”  

- - - -

#### Escenario \#15: `Importe` con símbolos.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** ingreso un símbolo  
**ENTONCES** el sistema muestra debajo del campo `Importe` el mensaje de error  “No se respeta el formato moneda.“  

- - - -

#### Escenario \#16: `Importe` sólo espacios. 
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** completo el campo `Importe` sólo con espacios  
**ENTONCES** el sistema muestra debajo del campo `Importe` el mensaje de error  “El campo es requerido“  