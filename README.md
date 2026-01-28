# Git y GitHub: Guía Completa

## ¿Qué es Git?

**Git** es un sistema de control de versiones distribuido, gratuito y de código abierto. Fue creado por Linus Torvalds en 2005 para el desarrollo del kernel de Linux. Git permite a los desarrolladores realizar un seguimiento de los cambios en su código a lo largo del tiempo, colaborar con otros y mantener un historial completo del proyecto.

### Características principales de Git:

- **Control de versiones**: Guarda instantáneas del proyecto en diferentes momentos
- **Distribuido**: Cada desarrollador tiene una copia completa del repositorio
- **Rápido y eficiente**: Operaciones locales muy rápidas
- **Ramificación**: Sistema de ramas ligero y flexible
- **Integridad**: Usa checksums SHA-1 para garantizar la integridad de los datos

## ¿Qué es GitHub?

**GitHub** es una plataforma de alojamiento de código basada en la nube que utiliza Git. Fue lanzada en 2008 y adquirida por Microsoft en 2018. GitHub proporciona una interfaz web para los repositorios Git y añade características de colaboración, gestión de proyectos y redes sociales para desarrolladores.

### Características principales de GitHub:

- **Hosting de repositorios**: Almacena repositorios Git en la nube
- **Colaboración**: Pull requests, code reviews, issues
- **GitHub Actions**: Automatización de CI/CD
- **GitHub Pages**: Hosting gratuito de sitios web estáticos
- **Seguridad**: Escaneo de vulnerabilidades y Dependabot
- **Comunidad**: Red social para desarrolladores

## Comandos básicos de Git

### Configuración inicial
```bash
# Configurar nombre de usuario
git config --global user.name "Tu Nombre"

# Configurar email
git config --global user.email "tuemail@ejemplo.com"

# Ver configuración
git config --list
```

### Crear y clonar repositorios
```bash
# Inicializar un nuevo repositorio
git init

# Clonar un repositorio existente
git clone https://github.com/usuario/repositorio.git
```

### Comandos básicos de trabajo
```bash
# Ver estado de los archivos
git status

# Añadir archivos al área de staging
git add archivo.txt
git add .  # Añadir todos los archivos

# Confirmar cambios
git commit -m "Mensaje descriptivo del commit"

# Ver historial de commits
git log
git log --oneline  # Versión compacta
```

### Trabajar con ramas
```bash
# Ver ramas
git branch

# Crear una nueva rama
git branch nombre-rama

# Cambiar a una rama
git checkout nombre-rama

# Crear y cambiar a una rama en un solo comando
git checkout -b nombre-rama

# Fusionar una rama con la actual
git merge nombre-rama

# Eliminar una rama
git branch -d nombre-rama
```

### Trabajar con repositorios remotos
```bash
# Ver repositorios remotos
git remote -v

# Añadir un repositorio remoto
git remote add origin https://github.com/usuario/repositorio.git

# Enviar cambios al repositorio remoto
git push origin main

# Obtener cambios del repositorio remoto
git pull origin main

# Obtener información sin fusionar
git fetch
```

## Flujo de trabajo típico con Git

1. **Inicializar o clonar** un repositorio
2. **Crear una rama** para tu nueva funcionalidad
3. **Hacer cambios** en los archivos
4. **Añadir cambios** al staging area con `git add`
5. **Confirmar cambios** con `git commit`
6. **Enviar cambios** al repositorio remoto con `git push`
7. **Crear un Pull Request** en GitHub (si trabajas en equipo)
8. **Revisar y fusionar** los cambios

## Diferencias entre Git y GitHub

| Git | GitHub |
|-----|--------|
| Software de control de versiones | Plataforma de hosting en la nube |
| Se instala localmente | Se accede vía web |
| Línea de comandos | Interfaz gráfica web |
| Maneja versiones de código | Añade colaboración y gestión de proyectos |
| Funciona sin conexión | Requiere conexión a internet |
| Gratuito y open source | Gratuito con opciones de pago |

## Conceptos importantes

### Commit
Una instantánea de los cambios en tu código en un momento específico. Cada commit tiene un identificador único (hash SHA-1).

### Branch (Rama)
Una línea independiente de desarrollo. Permite trabajar en nuevas características sin afectar el código principal.

### Merge
El proceso de combinar cambios de diferentes ramas.

### Pull Request
Una solicitud para fusionar cambios de una rama a otra. Permite revisión de código antes de la fusión.

### Fork
Una copia de un repositorio que permite experimentar sin afectar el proyecto original.

### Clone
Una copia local de un repositorio remoto.

## Buenas prácticas

1. **Commits frecuentes**: Realiza commits pequeños y frecuentes con mensajes descriptivos
2. **Mensajes claros**: Escribe mensajes de commit que expliquen el "qué" y el "por qué"
3. **Usa ramas**: Crea ramas para nuevas funcionalidades o correcciones
4. **Pull requests**: Usa PRs para revisión de código antes de fusionar
5. **Mantén actualizado**: Sincroniza regularmente con el repositorio remoto
6. **Archivo .gitignore**: Excluye archivos que no deben versionarse

## Recursos adicionales

- [Documentación oficial de Git](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com)
- [Pro Git Book](https://git-scm.com/book/es/v2) - Libro gratuito en español
- [GitHub Learning Lab](https://lab.github.com/)

## Conclusión

Git y GitHub son herramientas esenciales en el desarrollo de software moderno. Git proporciona el control de versiones potente y flexible, mientras que GitHub añade las herramientas de colaboración necesarias para trabajar en equipo. Dominar estas herramientas es fundamental para cualquier desarrollador.

---

*Última actualización: Enero 2026*
