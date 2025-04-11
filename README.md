# NestJS DDD Example

Este proyecto es una implementación de ejemplo de Domain-Driven Design (DDD) utilizando NestJS, siguiendo los principios de Arquitectura Hexagonal y CQRS.

## Estructura del Proyecto

```
src/
├── contexts/                # Contextos delimitados
│   └── user-management/    # Contexto de gestión de usuarios
│       ├── domain/        # Capa de dominio
│       ├── application/   # Capa de aplicación
│       └── infrastructure/# Capa de infraestructura
└── shared/                # Código compartido entre contextos
```

## Requisitos Previos

- Node.js (v14 o superior)
- PostgreSQL
- npm o yarn

## Configuración

1. Clonar el repositorio:
```bash
git clone https://github.com/jlortegacares/nestjs-ddd-example.git
cd nestjs-ddd-example
```

2. Instalar dependencias:
```bash
npm install
```

3. Configurar variables de entorno:
```bash
cp .env.example .env
# Editar .env con tus configuraciones
```

4. Crear la base de datos:
```bash
createdb ddd_example
```

## Ejecución

```bash
# desarrollo
npm run start:dev

# producción
npm run build
npm run start:prod
```

## Pruebas

```bash
# unit tests
npm run test

# e2e tests
npm run test:e2e

# test coverage
npm run test:cov
```

## Características

- Arquitectura DDD con contextos delimitados
- Implementación de CQRS
- Arquitectura Hexagonal
- TypeORM para la persistencia
- Validación de datos
- Manejo seguro de contraseñas
- Tests unitarios y de integración

## Licencia

MIT