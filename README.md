# Servidor SFTP + WebDAV

Práctica de servidores SFTP y WebDAV con Docker.

## Requisitos

- Docker (o Colima en macOS)
- Docker Compose

## Instalación

```bash
# Clonar el repositorio
git clone <tu-repo>
cd servidor_sftp_despligue

# Levantar servicios
docker compose up -d --build
```

## Acceso

**SFTP** (puerto 2222):
- alumno1 / Alumno123
- alumno2 / Alumno123  
- profesor / Profe123

**WebDAV** (puerto 8080):
- http://localhost:8080
- Credenciales en `webdav/htpasswd`

## Detener

```bash
docker compose down
```