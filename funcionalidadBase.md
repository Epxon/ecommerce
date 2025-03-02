# Funcionalidad de la base de datos

## Descripción
Base de datos creada en el entorno SQL para la manipulación de datos del software de  administración de un gimnasio

### Recursos utilizados
1. Procedure
1. Procedure con cursor
1. función sin parametros
1. funcion con parametros
1. Trigger simple
1. Trigger de borrado en cascada - **BEFORE**
1. Trigger de borrado en cascada - **AFTER**
1. Index

## Ejemplo implementación
| Metodo | Codigo | 
|-|-|
| Procedure | delimiter // create procedure paProductos() begin select * from producto end // delimiter // | 
| Funcion sin parametros | delimiter // create function HolaMundo() returns **VARCHAR(20)** as begin RETURN 'Hola mundo' ; END |
| Trigger simple | create trigger trgDespuesDeCliente on Clientes after INSERT AS BEGIN PRINT 'Se ha insertado un nuevo cliente en la tabla clientes' ; END |
| Index | create index idxNombreCliente on Clientes (Nombre); |



