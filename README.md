# Proyecto 1 — CI/CD con GitHub Actions y Docker

## Descripción
Proyecto práctico que implementa un pipeline de integración continua (CI) utilizando Python, GitHub Actions y Docker.

El objetivo es automatizar las pruebas de una aplicación Python y construir y ejecutar un contenedor Docker.

## Tecnologías utilizadas
- Python 3.12
- Pytest
- Git y GitHub
- GitHub Actions
- Docker

## Estructura del proyecto
```text
proyecto-github-actions/
├── .github/
│   └── workflows/
│       └── tests.yml
├── app.py
├── test_app.py
├── requirements.txt
├── Dockerfile
└── .gitignore
```

## Funcionamiento del pipeline
1. GitHub recibe los cambios del repositorio.
2. GitHub Actions activa el workflow.
3. Se instalan las dependencias.
4. Se ejecutan las pruebas automáticas con Pytest.
5. Se construye la imagen Docker.
6. Se ejecuta un contenedor Docker.
7. Se validan las pruebas dentro del contenedor.

## Ejecución local

Ejecutar las pruebas:
```bash
pytest
```

Construir la imagen:
```bash
docker build -t mi-aplicacion .
```

Ejecutar el contenedor:
```bash
docker run --rm mi-aplicacion
```

## Resultado
Se implementó exitosamente un pipeline CI que automatiza las pruebas y la construcción y ejecución de una aplicación Python mediante Docker.
