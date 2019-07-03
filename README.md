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

Referencias
 - [Developers-sw](https://developers.sw.com.mx/knowledge-base/servicio-publico-de-consulta-estatus-cfdi-sat/)
 - [Tar.mx](https://tar.mx/archivo/2018/validar-folio-fiscal-cfdi-con-php-directo-del-sat-2018.html)
 - [SAT](https://www.sat.gob.mx/consulta/71663/conoce-los-servicios-especializados-de-validacion) En esta liga se encuentra el manual en pdf (Web Service de Validación de CFDI)
