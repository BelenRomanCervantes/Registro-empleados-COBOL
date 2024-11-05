# Registro de empleados COBOL 
## Objetivo
Realizar un programa que permita registrar los empleados de una empresa en un archivo indexado. 
## Funcionamiento
El programa presenta un menú con las siguientes instrucciones:
```
INGRESAR UNA DE LAS SIGUIENTES OPCIONES: 
A: ALTAS 
I: IMPRIMIR
M: MODIFICAR
E: ELIMINAR
S: SALIR
```

### **Altas**
Permite capturar los siguientes datos:
*	Número de empleado (8 dígitos)
*	Nombre del empleado
    *	Nombre (20 caracteres)
    *	Primer apellido (20 caracteres)
    *	Segundo apellido (20 caracteres)
*	Fecha de nacimiento
    *	Año (4 dígitos)
    *	Mes (2 dígitos)
    *	Día (2 dígitos)
*	Sexo (1 carácter, M para mujer, H para hombre)
*	Domicilio (30 caracteres)
*	Teléfono (10 dígitos)
*	RFC (13 caracteres)
*	NSS (11 caracteres)
*	Sin uso (100 caracteres)

La captura será a través de una cadena. 
Cada dato estará separado por una coma.
El programa comprobará que ningún campo se encuentre vacío y que el número de empleado no esté duplicado.
Si todo es correcto, almacenará los datos en un archivo indexado. 

![image](https://github.com/user-attachments/assets/a93ddb3d-90e9-4dd5-9e67-9fa8b29cfbbd)

### **Imprimir**
Solicita el número de empleado cuya información se desea mostar en pantalla.
Se realiza la búsqueda de ese número de empleado.
Si dicho empleado se encuentra presente, se muestra un reporte con los datos del empleado. 

![image](https://github.com/user-attachments/assets/88662b2f-c6b6-4ead-99d7-9f4f6d11ca90)

### **Modificar**
Aparece un submenú con las siguientes opciones:
C: ACTUALIZAR CAMPOS NO LLAVE
L: ACTUALIZAR TODO EL REGISTRO INCLUIDO EL CAMPO LLAVE

En cualquiera de los 2 casos la actualización se hará por medio de una cadena donde se ingresan todos los datos modificados.
Cada dato estará separado por una coma.
Igual que en el proceso de alta, el programa comprobará que ningún campo se encuentre vacío y que el número de empleado no esté duplicado.

Al elegir la opción C, la cadena con los datos no debe incluir el número de empleado, ya que no desea modificarlo. 

![image](https://github.com/user-attachments/assets/74039b83-9a5c-474c-94b5-88c5d8d678a9)

Al elegir la opción L, el sistema solicitará confirmación para eliminar el registro actual y posteriormente solicitará los nuevos datos. 

![image](https://github.com/user-attachments/assets/6b6616b4-dc89-44d1-a610-4e2b09d796e8)

### **Eliminar**
Solicita el número de empleado cuya información se desea mostar en pantalla.
Se realiza la búsqueda de ese número de empleado.
Si dicho empleado se encuentra presente, se solicita confirmación para proceder con la eliminación del registro. 

![image](https://github.com/user-attachments/assets/249a6ae2-ea2b-4dec-a8fe-b2b1aeac4f1b)

### **Salir**
El programa es finalizado inmediatamente. 

![image](https://github.com/user-attachments/assets/82b64f5e-76c7-4670-bc52-5d8f3d9a9c25)

### **Opción inválida**
En caso de que el usuario ingrese una opción que no sea A, I, M, E o S, el programa lanza un mensaje de advertencia y el proceso vuelve a iniciar. 

![image](https://github.com/user-attachments/assets/03b948c0-d340-4241-be88-693829183a9e)
