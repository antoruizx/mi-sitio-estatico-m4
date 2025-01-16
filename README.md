## Desafío M4

Configuración para desplegar un sitio web estático utilizando S3 y CloudFront en AWS, con automatización a través de GitHub Actions.

## Pasos realizados

1. **Creación del sitio web**

Diseñé un sitio web estático con archivos index.html y error.html.

2. **Configuración de Amazon S3**

Creé un bucket S3 y habilité el alojamiento de sitios web estáticos.

Configuré las políticas de acceso para permitir que CloudFront acceda al contenido.

3. **Configuración de Amazon CloudFront**

Creé una distribución de CloudFront apuntando al bucket S3 como origen.

Configuré el objeto raíz predeterminado como index.html.

4. **Automatización con GitHub Actions**

Configuré un flujo de trabajo en GitHub Actions para sincronizar archivos con S3 y invalidar la caché de CloudFront tras cada cambio en la rama main.

Utilicé secretos para almacenar las credenciales de AWS.

5. **Pruebas y verificación**

Verifiqué que el sitio estático estuviera accesible desde la URL de CloudFront.

Realicé cambios en el código y validé que se reflejaran automáticamente en el sitio.

## Requisitos presentados

**Cuenta en AWS**,
**Cuenta en GitHub**,
**GitHub Actions configurado con secretos para las credenciales de AWS**.

