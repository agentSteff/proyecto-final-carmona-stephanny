🚀 Proyecto Final Git y GitHub
👤 Estudiante: Stephanny Carmona Campos

📝 Descripción
Este proyecto simula un entorno real de trabajo colaborativo usando Git y GitHub. El objetivo principal es practicar control de versiones, ramas, resolución de conflictos y documentación técnica bajo buenas prácticas profesionales.

📁 Estructura del Repositorio
README.md: Documentación principal del proyecto.

datos.xlsx: Tabla de datos (mínimo tres filas y columnas).

registro.txt: Lista de miembros y carreras, modificada para conflicto.

/imagenes: Carpeta con todas las capturas del flujo y conflicto.

👥 Miembros del equipo
Ana Rodríguez – Ingeniería en Sistemas

Luis Fernández – Diseño UX

María Leiva – Ingeniería Electrónica / Arquitectura / Ingeniería Civil

💻 Comandos utilizados
bash
cd "/c/Users/Usuario/proyecto-final-carmona-stephanny"
echo "# Proyecto Final Git y GitHub" > README.md
echo "**Estudiante:** Stephanny Carmona Campos" >> README.md
ls -l
rm -r README.md
git add datos.xlsx registro.txt
git commit -m "Agrega archivos de datos y registro iniciales"
git remote add origin https://github.com/agentSteff/proyecto-final-carmona-stephanny.git
git branch -M main
git push -u origin main
mkdir imagenes
git add imagenes/
git commit -m "Agrega carpeta para imágenes de capturas"
git add .
git commit -m "Agrega carpeta imagenes y actualiza README.md"
git push
git branch rama-A
git branch rama-B
git checkout rama-A
git add registro.txt
git commit -m "Modifica línea de María en rama-A"
git checkout rama-B
git add registro.txt
git commit -m "Modifica línea de María en rama-B"
git checkout main
git merge rama-A
git merge rama-B
git add registro.txt
git commit -m "Resolución final del conflicto en registro.txt"
git add imagenes/conflicto.png imagenes/estructura.png imagenes/gitrepo.png imagenes/resuelto.png
git commit -m "Agrega imágenes de evidencia finales"
git push
⚙️ Flujo de trabajo
Se crearon ramas desde main.

Ambas ramas modificaron la misma línea en registro.txt.

En el merge, Git detectó el conflicto y se resolvió combinando las versiones.

Todo el proceso fue documentado con capturas de pantalla.

🖼️ Evidencia visual
⚡️ Conflicto generado en registro.txt
✅ Resolución manual del conflicto
💼 Estructura del proyecto
🌐 Vista final en GitHub

💭 Reflexión personal
Durante la elaboración de este proyecto, enfrenté retos al estructurar el repositorio y organizar las ramas. Aprendí a documentar cada paso, comprobar archivos antes de hacer commit y a resolver conflictos manualmente por misma, comprendiendo cómo Git me facilita la integración de cambios. El ejercicio me fortalece la colaboración y me fomenta la disciplina para proyectos reales de desarrollo queme encuentro actualmente.
