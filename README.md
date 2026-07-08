# Gestion de Vacaciones QA - eCommerce Aeromexico

## Setup GitHub Pages

### Paso 1: Crear repositorio en GitHub
1. Ir a https://github.com/new
2. Nombre: `vacaciones-qa`
3. Visibilidad: Public (para GitHub Pages gratis)
4. Crear repositorio

### Paso 2: Subir archivos
```bash
cd vacaciones-qa-app
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/jsantillan_amx/vacaciones-qa.git
git branch -M main
git push -u origin main
```

### Paso 3: Activar GitHub Pages
1. Ir a Settings > Pages en el repo
2. Source: Deploy from a branch
3. Branch: main, folder: / (root)
4. Save

En 1-2 minutos estara disponible en:
`https://jsantillan_amx.github.io/vacaciones-qa/`

### Paso 4: Compartir URL con el equipo
Compartir la URL de GitHub Pages. Todos veran los datos del `data.json`.

## Como registrar vacaciones

Editar `data.json` directamente en GitHub (o via Kiro):

```json
{
  "vacations": [
    {"date":"2025-07-15","person":"Eduardo Colin Hernandez","type":"V","backup":"Violeta Troncoso Reyes"},
    {"date":"2025-07-16","person":"Eduardo Colin Hernandez","type":"V","backup":"Violeta Troncoso Reyes"}
  ],
  "history": [
    {"requestDate":"2025-07-08","person":"Eduardo Colin Hernandez","dates":"15-Jul, 16-Jul","type":"V","backup":"Violeta Troncoso Reyes","chapter":"Jose Alfonso Santillan Rosete","status":"Aprobado"}
  ]
}
```

Despues de hacer commit, la pagina se actualiza automaticamente en ~1 min.

## Permisos
- **Anet + Chapter Leads**: colaboradores del repo (pueden editar data.json)
- **Resto del equipo**: solo visualizan la URL publica

## Estructura
- `index.html` - Aplicacion principal
- `data.json` - Datos compartidos (vacaciones, historial, fechas bloqueadas)
- `logo.jpg` - Logo (opcional)
