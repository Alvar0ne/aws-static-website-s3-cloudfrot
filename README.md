# Proyecto AWS: Despliegue de Sitio Web Estático con Amazon S3 y CloudFront
Este proyecto consiste en la implementación de una arquitectura serverless para alojar un sitio web estático utilizando servicios de Amazon Web Services (AWS).
La solución utiliza Amazon S3 para el almacenamiento y publicación de archivos HTML, CSS e imágenes, mientras que Amazon CloudFront se encarga de distribuir el contenido mediante una red global de entrega (CDN), mejorando el rendimiento y reduciendo la latencia para los usuarios.


## Objetivo

Implementar una solución de alojamiento web de bajo costo, alta disponibilidad y sin necesidad de administrar servidores, aplicando conceptos fundamentales de computación en la nube.



## Arquitectura

Usuario

↓

Amazon CloudFront (CDN)

↓

Amazon S3 (Static Website Hosting)


Imagen de arquitectura

(INSERTAR IMAGEN: architecture-diagram.png)


## Servicios AWS Utilizados

### Amazon S3

Servicio de almacenamiento de objetos utilizado para:

Almacenar archivos HTML
Almacenar hojas de estilo CSS
Almacenar imágenes y recursos estáticos
Publicar contenido web estático
Amazon CloudFront

### Servicio CDN utilizado para:

Distribuir contenido globalmente
Reducir tiempos de carga
Almacenar contenido en caché
Entregar contenido mediante HTTPS


## Implementación


1. Creación del Bucket S3

Se creó un bucket dedicado para almacenar los archivos del sitio web.

(INSERTAR IMAGEN: s3-bucket-created.png)



2. Carga de Archivos

Se cargaron los archivos del sitio:

index.html
CSS
Imágenes
Recursos estáticos

(INSERTAR IMAGEN: s3-objects.png)


3. Configuración de Static Website Hosting

Se habilitó el alojamiento web estático dentro de Amazon S3 y se configuró el documento principal:

index.html

(INSERTAR IMAGEN: static-website-hosting.png)


4. Configuración de CloudFront

Se creó una distribución de CloudFront utilizando el bucket S3 como origen del contenido.

(INSERTAR IMAGEN: cloudfront-config.png)

5. Validación del Despliegue

Se verificó el acceso exitoso al sitio mediante la URL generada por CloudFront.

(INSERTAR IMAGEN: deployment-success.png)

## Habilidades Aplicadas

AWS Cloud Computing
Amazon S3
Amazon CloudFront
Object Storage
CDN
Static Website Hosting
Arquitectura Serverless
Publicación de aplicaciones web
Gestión de contenido estático
Optimización de rendimiento web


## Beneficios de la Solución


Bajo costo operativo
Alta disponibilidad
Escalabilidad automática
Distribución global de contenido
Sin administración de servidores
Arquitectura moderna basada en servicios administrados



## Aprendizajes Obtenidos


Durante este proyecto se adquirieron conocimientos prácticos sobre:

Funcionamiento de Amazon S3 como alojamiento web estático.
Uso de CloudFront como red de distribución de contenido (CDN).
Relación entre almacenamiento de objetos y entrega de contenido.
Arquitecturas serverless para aplicaciones web.
Implementación de soluciones cloud de bajo costo.


## Tecnologías Utilizadas

Amazon S3
Amazon CloudFront
HTML5
CSS3
AWS Management Console


## Mejoras Futuras

Implementación de dominio personalizado.
Configuración de Route 53.
Integración con AWS Certificate Manager (ACM).
Automatización mediante GitHub Actions.
Implementación utilizando Terraform o CloudFormation.
