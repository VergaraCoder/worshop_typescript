# worshop_typescript
Este pequeño programa es el encargado de la gestion de un inventario de medicamentos que usa para su estructura e modelo MVC, que se encarga de :

_____________________________________________________________

-Mostrar todos los medicamentos que estan en la base de datos . --> get (http://localhost:3001/farmacia/medices)

_______________

-Mostrar un medicamento especifico -->             get(http://localhost:3001/farmacia/medices/1)

______________

-Enviar un nuevo medicamento --> OBJETO ESPECIFICO PARA MANDAR --> 
medicamento{
    nombre:string,
    cantidad:number,
    fecha_caducidad:string,
    precio:number
}
El endopint para mandar nuevo medicamento es          post(http://localhost:3001/farmacia/medices)

___________________

-Actualizar la cantidad de un medicamento --> OBJETO ESPECIFICO A MANDAR --> 
actualizar {
  "cantidad": numero a actualizar
}

EL endopint para actualizar la cantidad es     put(http://localhost:3001/farmacia/medices/id)

___________________

Eliminar un medicamento en especifico --> NO HAY QUE MANDAR NINGUN OBJETO , TODO ES POR LOS PARAMETROS DE URL

El endopint para eliminar medicamento en especifico es     delete(http://localhost:3001/farmacia/medices/id)

_____________________________________________________________________________________________________



COMANDOS PARA INICIAR PROYECTO 

tsc --watch --> para estar atento a cada cambio que se haga nuevo en los archivos .ts

npm start --> para mostrar los cambios compilados en js , este comando en el que verdaderamente hace funcionar al proyecto


_____________________________________________________________________________________

POSIBLES ERRORES 

Al momento de compilar los archivos a .js , y usar import y export , se suponia que los archivos desde los .ts se les pone la ruta relativa (ES DECIR SIN PONER EL .TS ) y ya en la compilacion ya el programa mismo le agregaria el .js , pero no fue asi , y me toco poner a todos los archivos compilados a js , la extension.js 

Por lo que lo que si se vuelve a compilar los .ts , posiblemente los arhcivos .js vuelvan a tener la ruta relativa , por lo que abria que volver a poner a todos los archvos importados que estan dentro del mimso proyecto el .js (SOLO A LOS COMPILADOS , LOS ARCHIVOS .TS SE DEJAN TAL CUAL)



______________________________

DESDE QUE CARPETA ABRIR EL PROYECTO?

Hacer el code . en la carpeta practice_typescript2

