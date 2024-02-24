Movi la ruta /api/users/premium/:uid a users
Modifique el userModel para que muestre los documentos cargados del usuario y un last_connection

Un api/users/:uid/documents que permite subir multiples archivos
    si es profileImage se guarda en /public/images/profiles
    si es productsImage se guarda en /public/images/products
    si es otro tipo se guarda en /public/documents

Multer donde selecciona la carpeta correspondiente y guarda el archivo con el id del usuario

El endpoint /api/users/premium/:uid solo actualiza a premium si el usuario tiene cargado los archivos correspondientes(identificacion, comprobante_domicilio, comprobante_estado_cuenta) y en caso de ser premium se puede volver a cambiar a usuario sin requerimientos 

