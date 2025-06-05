# Travelsiones

Aplicación móvil para turistas en Misiones, Argentina. Su objetivo es informar y guiar a los viajeros locales e internacionales a lo largo de su travesía.

## Folder Structure

The project follows a simple Clean Architecture layout:

- `src/domain` – entities and business logic
- `src/application` – use cases and application services
- `src/infrastructure` – external service implementations
- `src/presentation` – Angular components and routing

## Características principales
- Los usuarios establecen un punto de salida y de llegada, la cantidad de días de viaje y el tipo de recorrido (directo o con paradas).
- Con esa información, la app recomienda atracciones, cabañas, restaurantes y otros lugares de interés.
- También sugiere paradas en la ruta o dentro de un radio específico de kilómetros para enriquecer la experiencia.
- Busca resolver la falta de marketing y guía turística en la región de Misiones.

## Desarrollo

Este proyecto está construido con [Angular](https://angular.io). Para comenzar con el desarrollo local, ejecute:

```bash
ng serve
```

Abra el navegador en `http://localhost:4200/` para ver la aplicación. Los cambios en el código recargarán la página automáticamente.

Para compilar la aplicación ejecute:

```bash
ng build
```

Los artefactos de producción se generarán en la carpeta `dist/`.

Para ejecutar pruebas unitarias:

```bash
ng test
```

Si desea ejecutar pruebas end-to-end (e2e):

```bash
ng e2e
```

Para obtener más información sobre Angular CLI consulte la [documentación oficial](https://angular.dev/tools/cli).


## Arquitectura

El proyecto sigue una organización basada en los principios de _Clean Architecture_. Dentro de `src/app` se definen tres carpetas principales:

- `features/` alberga las **vistas** o páginas de la aplicación.
- `shared/components/` contiene los **componentes reutilizables**.
- `core/services/` incluye los **servicios** que encapsulan la lógica de negocio.

Esta estructura separa responsabilidades y facilita el mantenimiento del código.

