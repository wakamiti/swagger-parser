# Swagger Parser Shaded

Este proyecto proporciona una versión unificada (shaded) de `swagger-parser` v2.1.26 para resolver conflictos de  
nombres de módulos en entornos Java 9+.

## Propósito

Evitar el error de módulos duplicados al usar `swagger-parser` junto con otras dependencias que incluyan versiones  
antiguas (ej. v1.x):
```
Module 'swagger.parser' is already on the module path!
```

## Características

- **Nombre de módulo explícito**: Define `Automatic-Module-Name: io.swagger.parser`.
- **Unificación de dependencias**: Incluye todas las clases de `io.swagger` en un único JAR.
- **Compatibilidad**: Mantiene la funcionalidad de `swagger-parser` v2.1.26 para trabajar con OpenAPI v3 y Swagger v2.

