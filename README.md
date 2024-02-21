# VTEX B2B BILL

Como proceso de optimizacion en los sitios se estandrizó la implementación de formularios para facturación B2B

## Configuración

### Paso 1 - Instalar aplicación
En su cuenta .myvtex instalar la siguiente aplicación

```
 vtex install summasolutions.billing@0.1.0-beta.6
```

Esta aplicación habilitará un endpoint que ayudará a facilitar la configuración inicial

### Paso 2 - Correr enpoint

Ejecutar un *POST* a

```
 https://{{accountname}}.myvtext.com/billing
```

Esto generará los customData necesarios para que el formulario funcione correctamente.

### Paso 3 - Importar el script 

Agregar el siguiente código en su checkout

```
 $.getScript({{url del script necesario}})
```