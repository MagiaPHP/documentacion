# add.php  

## Plugin : Types 
## controllers : add.php 
##
  
Url doc: http://magiaphp.com/docs/001/types/controllers/add.php 

Fecha de creacion del documento: 2024-08-17 19:08:50 

Documento accesible via la siguiente url:  

`
if (!permissions_has_permission($u_rol, $c, "create")) {    
    header("Location: index.php?c=home&a=no_access");    
    die("Error has permission ");
}

include view("types", "add"); 
`



1) Verificamos si el `$u_rol` en `$c` tiene permiso para `create` 

if (!permissions_has_permission($u_rol, $c, "create")) {


    header("Location: index.php?c=home&a=no_access");

    #mg y matamos el proceso 

    die("Error has permission ");
}

#mg 2) si ha pasado el control anterior, incluimos la vista `add`                

include view("types", "add");

http://localhost/index.php?c=types&a=add 

