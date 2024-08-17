#add.php  

http://magiaphp.com 

Fecha de creacion del documento: 2024-08-17 19:08:48 

Documento accesible via la siguiente url:  
Verificamos si el `$u_rol` en `$c` tiene permiso para `create` 

`if (!permissions_has_permission($u_rol, $c, "create")) {`

    si no tiene permiso lo redireccionamos 
    
    `header("Location: index.php?c=home&a=no_access");`
    
    y matamos el proceso 

`die("Error has permission ");`
    
`}`

si ha pasado el control anterior, incluimos la vista `add`                

`include view("types", "add");`   http://localhost/index.php?c=types&a=add 

