# DG TALLER - DEPLOY GITHUB PAGES - INSTRUCCIONES PRECISAS

## CREDENCIALES
- Técnico: usuario **tecnico1** / contraseña **dg123**
- Cliente fija: código **ABC1234**

## ESTRUCTURA DEL ZIP (3 apps + root)
/
├── index.html (landing que enlaza a las 3 apps)
├── manifest.json
├── README.md (este archivo)
├── supervisor/index.html
├── tecnico/index.html
├── cliente/index.html
├── contrato/index.html
└── icons/ (iconos PWA)

## PASO A PASO GITHUB - 100% PRECISO

### 1. Crear repo
1. Entra a github.com > New repository
2. Nombre: dg-taller (público)
3. NO inicialices con README
4. Create repository

### 2. Subir ZIP descomprimido (método más fácil, sin git)
1. Descomprime dg-taller-github.zip en tu PC
2. En GitHub, dentro del repo vacío, click **Add file** > **Upload files**
3. **ARRASTRA TODA LA CARPETA DESCOMPRIMIDA**: arrastra los archivos y CARPETAS (supervisor, tecnico, cliente, contrato, icons) + index.html + manifest.json
   - IMPORTANTE: GitHub permite arrastrar carpetas directamente desde 2023. Si no te deja, arrastra carpeta por carpeta.
4. Espera que suba todo (debe verse supervisor/index.html etc en la lista)
5. Scroll abajo, escribe Commit message: "Deploy inicial DG Taller"
6. Click **Commit changes**

### 3. Activar Pages
1. Ve a Settings > Pages (barra lateral izquierda)
2. En Build and deployment > Source: **Deploy from a branch**
3. Branch: **main** / root > Save
4. Espera 1-2 minutos. Refresca.
5. Arriba te mostrará: **Your site is live at https://TUUSUARIO.github.io/dg-taller/**

### 4. URLs finales
- Landing: https://TUUSUARIO.github.io/dg-taller/
- Supervisor: https://TUUSUARIO.github.io/dg-taller/supervisor/
- Técnico: https://TUUSUARIO.github.io/dg-taller/tecnico/
- Cliente: https://TUUSUARIO.github.io/dg-taller/cliente/ (probar con ABC1234)
- Contrato: https://TUUSUARIO.github.io/dg-taller/contrato/

### 5. Actualizar archivos luego
- Para reemplazar un index.html: entra a esa carpeta en GitHub > Add file > Upload files > arrastra el nuevo index.html > Commit (tildar overwrite)
- O edita directo: click en el archivo > lápiz > pega nuevo código > Commit

### TROUBLESHOOTING
- Si cliente no abre: verifica que cliente/index.html exista en main branch, no dentro de otra subcarpeta.
- Si Pages no carga: Settings > Pages debe decir Branch: main. Si dice None, selecciona main.
- Cache: probá en incógnito o ?v=2 al final de la URL.

## NOTAS
- Este ZIP ya incluye templates funcionales probados con ABC1234 y tecnico1/dg123
- Si tenés los HTML finales reales de tus artifacts, pégalos en los textareas del Armador antes de generar el ZIP para que los incluya.
- Icons son placeholders; podés reemplazarlos por tus logos.

Hecho con ❤️ - DG Taller Armador v1
