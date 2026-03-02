# leliasierra

¡Hola mundo!

## Comandos para crear este repositorio

### 1. Inicializar repositorio local
```bash
git init
git config user.name "<YOUR_USERNAME>"
git config user.email "<YOUR_EMAIL>"
```

### 2. Crear archivo README
```bash
echo "# <REPO_NAME>" > README.md
```

### 3. Hacer commit inicial
```bash
git add README.md
git commit -m "Initial commit: Hello World"
```

### 4. Crear repositorio remoto en GitHub
```bash
gh repo create <REPO_NAME> --source=. --remote=origin --push --public
```

### 5. Agregar remoto y hacer push (si es necesario)
```bash
git remote add origin git@github.com:<USERNAME>/<REPO_NAME>.git
git push -u origin master
```

## Requisitos previos

- Git instalado
- GitHub CLI (gh) instalado
- SSH configurado en GitHub
- Autenticado con `gh auth login`

## Clonar este repositorio

```bash
git clone git@github.com:<USERNAME>/<REPO_NAME>.git
```
