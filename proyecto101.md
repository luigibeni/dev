# Proyecto Controlador Hidropónico 

Este es un resumen general del proyecto que vamos a desarrollar y desplegar para un controlador basado en Arduino para controlar un sistema hidropónico.

## Tecnologias

### Esquema básico del sistema

El sistema va a estar compuesto por los siguientes elementos que serán explicados detalladamente más adelante.

1. Controlador arduino el cual tendrá cargado un scketch para comunicarse por el puerto serie con el PC o Raspberry Pi que contiene el backend.

2. Backend en Python a en modo servidor el cual estará conectado fisicamente al arduino y se encargará de recibir de este diferentes parametros como temperatura, humedad, ec y ph. Guardará todo en una base de datos y tambien se enviará al arduino instrucciones para activar o desactivar relés y demás actuadores emcargados de encender o apagar las bombas de riego, etc.

3. Frontend desarrollado en React para que el usuario pueda ver información en tiempo real y el pasado sobre el estado del sistema, y activar o activar de manera manual o automática los actuadores.
Se comunicará con el backend a través de una API.
4. Base de datos

### Backend

Para el back