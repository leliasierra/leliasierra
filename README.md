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

### 1. Instalar Git

#### En Windows (usando Chocolatey)
```powershell
choco install git
```

#### En Windows (usando Scoop)
```powershell
scoop install git
```

#### En macOS
```bash
brew install git
```

#### En Linux (Ubuntu/Debian)
```bash
sudo apt-get install git
```

### 2. Instalar GitHub CLI

#### En Windows (usando Winget)
```powershell
winget install --id GitHub.cli -e --silent --accept-package-agreements --accept-source-agreements
```

#### En Windows (usando Chocolatey)
```powershell
choco install gh
```

#### En macOS
```bash
brew install gh
```

#### En Linux
```bash
sudo apt-get install gh
```

### 3. Configurar SSH

#### Generar clave SSH
```bash
ssh-keygen -t rsa -b 4096 -f ~/.ssh/id_rsa -N ""
```

En Windows (PowerShell):
```powershell
ssh-keygen -t rsa -b 4096 -f "$env:USERPROFILE\.ssh\id_rsa" -N ""
```

#### Ver tu clave pública
```bash
cat ~/.ssh/id_rsa.pub
```

En Windows (PowerShell):
```powershell
Get-Content "$env:USERPROFILE\.ssh\id_rsa.pub"
```

#### Agregar clave SSH a GitHub
1. Ve a https://github.com/settings/keys
2. Haz clic en "New SSH key"
3. Pega el contenido de tu clave pública
4. Dale un nombre descriptivo (ej: "Mi PC")
5. Guarda

#### Verificar conexión SSH
```bash
ssh -T git@github.com
```

Deberías ver: `Hi <USERNAME>! You've successfully authenticated, but GitHub does not provide shell access.`

### 4. Autenticar GitHub CLI

```bash
gh auth login
```

Selecciona:
- `GitHub.com` (para GitHub.com)
- `SSH` (protocolo preferido)
- `<YOUR_SSH_KEY>` (tu clave SSH)
- `Login with a web browser` (autenticación)

## Clonar este repositorio

```bash
git clone git@github.com:<USERNAME>/<REPO_NAME>.git
```
