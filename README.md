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

## Paquete nuget
- [Descargue el paquete nuget](https://www.nuget.org/packages/CFDI-SAT)

## Ejemplo en C#, 

```
using System;
using System.Web.UI;
using SesverSAT;

namespace WebApplication1
{
    public partial class _Default : Page
    {
        protected void Page_Load(object sender, EventArgs e)
        {
            ConsultaWebNa consultaSAT = new ConsultaWebNa();
            var respuesta = consultaSAT.ConsultaCFDI("LSO1306189R5", "GACJ940911ASA", "4999.99", "e7df3047-f8de-425d-b469-37abe5b4dabb");
            string estado = respuesta.Estado;
        }
    }
}
```


## Contacto

```
fdominguezg@hotmail.com
Software developer
```

Referencias
 - [Developers-sw](https://developers.sw.com.mx/knowledge-base/servicio-publico-de-consulta-estatus-cfdi-sat/)
 - [Tar.mx](https://tar.mx/archivo/2018/validar-folio-fiscal-cfdi-con-php-directo-del-sat-2018.html)
 - [SAT](https://www.sat.gob.mx/consulta/71663/conoce-los-servicios-especializados-de-validacion) En esta liga se encuentra el manual en pdf (Web Service de Validación de CFDI)
