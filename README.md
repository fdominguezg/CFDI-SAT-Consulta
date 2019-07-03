# CFDI-SAT

Esta es una libreria que ayuda a consultar el estatus de un CFDI (factura) ante el SAT.

## Como utilizarla

- Esta clase utiliza el API del SAT para conocer el estado de las facturas

    - El nombre de la clase es ConsultaWebNa.
    - El metodo a utilizar se llama ConsultaCFDI
    - Consumir el metodo ConsultaCFDI como se muestra en la siguiente linea
    -   ConectaSAT.ConsultaCFDI("emisor", "receptor", "importe","CFDI")
            
            El resultado contiene los siguientes campos
                - Cancelado - Boolean
                - CodigoEstatus - String
                - EsCancelable -  String
                - Estado - String
                - EstatusCancelacion - String
                - ExpresionErronea - String
                - Vigente  - Boolean
            Francisco 03/07/2019


## Contacto

```
fdominguezg@hotmail.com
Software developer
```
