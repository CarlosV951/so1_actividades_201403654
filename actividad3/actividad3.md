# Actividad 3 - Gestión de Permisos
Crear un md file y resolver cada uno de los items solicitados a continución. Debe de colocar el comando utilizado asi como el resultado de este si es necesario. 

## Gestión de Usuarios

### Creación de Usuarios
Crea tres usuarios llamados `usuario1`, `usuario2` y `usuario3`.
| Comando | Salida |
| ------- | ------ |
| sudo useradd usuario1 | - |
| sudo useradd usuario2 | - |
| sudo useradd usuario3 | - |

### Asignación de Contraseñas
Establece una nueva contraseñas para cada usuario creado.
| Comando | Salida |
| ------- | ------ |
| sudo passwd usuario1 | Nueva contraseña:  <br> Vuelva a escribir la nueva contraseña:  <br> passwd: contraseña actualizada correctamente <br> |
| sudo passwd usuario2 | Nueva contraseña:  <br> Vuelva a escribir la nueva contraseña:  <br> passwd: contraseña actualizada correctamente <br> |
| sudo passwd usuario3 | Nueva contraseña:  <br> Vuelva a escribir la nueva contraseña:  <br> passwd: contraseña actualizada correctamente <br> |

### Información de Usuarios
Muestra la información de `usuario1` usando el comando `id`
| Comando | Salida |
| ------- | ------ |
| id usuario1 | uid=1001(usuario1) gid=1001(usuario1) grupos=1001(usuario1) |
| id usuario2 | uid=1002(usuario1) gid=1002(usuario2) grupos=1002(usuario2) |
| id usuario3 | uid=1003(usuario1) gid=1003(usuario3) grupos=1003(usuario3) |

### Eliminación de Usuarios
Elimina `usuario3`, pero conserva su directorio principal.
| Comando | Salida |
| ------- | ------ |
| sudo userdel usuario3 | - |

## Gestión de Grupos

### Creación de Grupos
Crea dos grupos llamados `grupo1` y `grupo2`.
| Comando | Salida |
| ------- | ------ |
| sudo groupadd grupo1 | - |
| sudo groupadd grupo2 | - |

### Agregar Usuarios a Grupos
Agrega `usuario1` a `grupo1` y `usuario2` a `grupo2`.
| Comando | Salida |
| ------- | ------ |
| sudo usermod -a -G grupo1 usuario1 | - |
| sudo usermod -a -G grupo2 usuario2 | - |

### Verificar Membresía
Verifica que los usuarios han sido agregados a los grupos utilizando el comando `groups`.
| Comando | Salida |
| ------- | ------ |
| groups usuario1 | usuario1 : usuario1 grupo1 |
| groups usuario2 | usuario2 : usuario2 grupo2 |

### Eliminar Grupo
Elimina `grupo2`.
| Comando | Salida |
| ------- | ------ |
| sudo groupdel usuario1 | - |

## Gestión de Permisos


### Creación de Archivos y Directorios


