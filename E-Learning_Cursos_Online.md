<a name="Inicio"></a>    
# Limpieza de datos - E-Learning Cursos Online [![Texto](https://user-images.githubusercontent.com/116538899/231064143-c080de13-8be9-4321-8694-e62539263f5a.png)](#Tabla-de-contenido2) ([ES](https://github.com/HansAllTech/Hans_Data_Analysis_Portfolio/edit/main/E-Learning_Cursos_Online.md) | [EN](https://github.com/HansAllTech/Hans_Data_Analysis_Portfolio/edit/main/E-Learning_Cursos_Online.md))
  
<p align = 'center'><img src="https://user-images.githubusercontent.com/116538899/235765262-8acfe1d1-a637-4ef7-adeb-b1880368c671.jpg" width ="25%"></p>
  
  
  
<a name="Tabla-de-contenido2"></a>
## Tabla de Contenido [![Texto](https://user-images.githubusercontent.com/116538899/231064143-c080de13-8be9-4321-8694-e62539263f5a.png)](#Tabla-de-contenido2)
- [Problema de negocio](#Problema)
- [Objetivo](#Objetivo2)
- [Diagrama](#Diagrama2)
- [Análisis Previo](#Análisis-Previo2)   
- [Análisis de Ventas](#Análisis-de-Ventas2)
- [Análisis de Tráfico Web](#Análisis-de-Tráfico-Web2)
- [Análisis Avanzado](#Análisis-Avanzado2)
- [Dashboard](#Visualización-en-Looker2)   
- [Conclusiones](#Conclusiones2) 
- [Recomendaciones](#Recomendaciones2)   


<a name="Problema"></a>    
## Problema de negocio [![Texto](https://user-images.githubusercontent.com/116538899/231064143-c080de13-8be9-4321-8694-e62539263f5a.png)](#Tabla-de-contenido2)
<p align='justify'>
El problema de negocio de LearnData es que actualmente no tiene un sistema establecido para capturar, analizar y tomar decisiones basadas en sus principales métricas financieras. Sin contar con un sistema eficaz, la empresa no puede identificar las áreas que necesitan mejoras o tomar decisiones informadas que impulsen el crecimiento de la empresa. Además, sin un proceso de captura de datos adecuado, los datos en crudo generados por la web del negocio podrían estar incompletos, ser inexactos o contener duplicados, lo que dificultaría aún más el análisis y la toma de decisiones.
</p>  
  
<a name="Objetivo2"></a>
## Objetivo [![Texto](https://user-images.githubusercontent.com/116538899/231064143-c080de13-8be9-4321-8694-e62539263f5a.png)](#Tabla-de-contenido2)
Realizar una limpieza de datos para asegurar que los datos en crudo relacionados con clientes, pagos, pedidos y productos estén completos, sean precisos y no contengan duplicados, lo que permitirá una mayor precisión en el análisis y una toma de decisiones más informada en cuanto a la gestión de clientes y ventas. Además, la empresa debe invertir en el desarrollo e implementación de un sistema que pueda capturar y analizar estos datos de manera eficiente y efectiva para que la empresa pueda tomar decisiones informadas y basadas en datos para mejorar su desempeño en términos de gestión de clientes y ventas.
</p>

<a name="Diagrama2"></a>
## Diagrama [![Texto](https://user-images.githubusercontent.com/116538899/231064143-c080de13-8be9-4321-8694-e62539263f5a.png)](#Tabla-de-contenido2)
<p align="center"><img src="https://user-images.githubusercontent.com/116538899/235769297-9446a0b7-0ce3-47b4-b7dd-0b3eac8e6c61.png" width= 60% height=60%></p>    
 
 
<a name="Análisis-Previo2"></a>
## Análisis Previo [![Texto](https://user-images.githubusercontent.com/116538899/231064143-c080de13-8be9-4321-8694-e62539263f5a.png)](#Tabla-de-contenido2)
1. ¿Que fuentes de datos tiene la empresa?
   <p align='justify'>La empresa utiliza wordpress con un plugin de wocommerce como plataforma de venta de sus cursos online y luego cuenta con stripe como pasarela de pagos a de más de los pagos de tarjeta de crédito.</p>
2. ¿En que formato se descargan los datos?    
   <p align='justify'> Los datos crudos los tendremos en csv directamente descargados de las fuentes.</p>
3. ¿Que datos tenemos?    
   <p align='justify'>Tenemos datos de los productos osea cursos que se venden, los clientes, de los pedidos y de los pagos recibidos por stripe.</p>
4. Modelo de datos    
   <p align='justify'>Tenemos la tabla de pedidos que se relaciona con la de clientes y productos mediante SKU_producto e id_cliente y por otro lado tenemos la tabla      la de pagos de stripe que la relacionaremos con la de pedidos por el numero de pedido.</p><br>   
5. Análisis exploratorio de las tablas.