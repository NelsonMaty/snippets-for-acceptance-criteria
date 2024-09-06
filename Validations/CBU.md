# CBU
#input


#### Escenario \#10: `CBU` válido.  
**DADO** un administrador en la pantalla `{pantalla}`  
**Y** completo el campo `CBU` con un valor numérico entero positivo de largo 22  
**CUANDO** quito el foco del campo  
**ENTONCES** el sistema no presenta ningún mensaje de error debajo del campo `CBU`  

- - - -

#### Escenario \#11: `CBU` alfanumérico.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** ingreso una letra en el campo CBU  
**ENTONCES** el sistema muestra debajo del campo `CBU` el mensaje de error “El campo debe contener solo caracteres numéricos.“  

- - - -

#### Escenario \#12: `CBU` numérico menor a 22 caracteres.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** ingreso valor numérico entero positivo de largo 21 en el campo CBU  
**ENTONCES** el sistema muestra debajo del campo `CBU` el mensaje de error “El campo debe contener 22 caracteres.“  

- - - -

#### Escenario \#13: `CBU` numérico mayor a 22 caracteres.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** ingreso valor numérico entero positivo de largo 21 en el campo CBU  
**ENTONCES** el sistema muestra debajo del campo `CBU` el mensaje de error “El campo debe contener 22 caracteres.“  

- - - -

#### Escenario \#14: `CBU` sin completar.  
**DADO** un administrador en la pantalla `{pantalla}`  
**Y** dejo el campo `CBU` sin completar  
**Y** completo los demás campos del formulario con información válida  
**CUANDO** presiono `GUARDAR`  
**ENTONCES** el sistema previene la carga mostrando en el campo `CBU` el mensaje “El campo es requerido”  

- - - -

#### Escenario \#15: `CBU` con símbolos.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** ingreso un símbolo  
**ENTONCES** el sistema muestra debajo del campo `CBU` el mensaje de error  “El campo debe contener solo caracteres numéricos.“  

- - - -

#### Escenario \#16: `CBU` sólo espacios.  
**DADO** un administrador en la pantalla `{pantalla}`  
**CUANDO** completo el campo `CBU` sólo con espacios  
**ENTONCES** el sistema muestra debajo del campo `CUIT` el mensaje de error  “El campo debe contener solo caracteres numéricos.“  