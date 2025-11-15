Proyecto Final Git y GitHub
Estudiante: Stephanny Carmona Campos

Descripción
Este proyecto simula un escenario real de trabajo colaborativo utilizando Git y GitHub. El objetivo fue aplicar conceptos de control de versiones, manejo de ramas, resolución de conflictos y documentación técnica, siguiendo una estructura profesional y buenas prácticas recomendadas en la industria.

Estructura del Repositorio
README.md: Documentación principal del proyecto.

datos.xlsx: Archivo de datos con al menos tres filas y tres columnas.

registro.txt: Lista de miembros y carreras, modificado para provocar un conflicto.

/imagenes: Carpeta con capturas del conflicto y su resolución.

Miembros del equipo
Ana Rodríguez – Ingeniería en Sistemas

Luis Fernández – Diseño UX

María Leiva – Ingeniería Electrónica / Arquitectura / Ingeniería Civil

Comandos utilizados
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
git commit -m "Agrega las imágenes de evidencia con nombres normalizados"
git push
Flujo de trabajo
Para demostrar el manejo de conflictos en Git, se crearon dos ramas desde main. En ambas se modificó la misma línea en registro.txt (carrera de María Leiva). Al fusionarlas en main, Git detectó el conflicto y se resolvió manualmente integrando todas las especialidades en una sola línea. El proceso fue documentado paso a paso con capturas.

Evidencia visual
Conflicto generado en registro.txt
Resolución manual del conflicto
Estructura del proyecto en Windows
Repositorio en GitHub
Reflexión personal
Durante la elaboración de este proyecto, enfrenté varios retos relacionados con la estructura del repositorio y la correcta gestión de ramas. Aprendí la importancia de documentar cada paso, verificar el estado de los archivos antes de hacer commits y cómo los conflictos surgen cuando varias ramas modifican la misma sección de un archivo. Resolver el conflicto manualmente permitió entender a profundidad cómo Git marca y permite fusionar ediciones sin perder información. Considero que este ejercicio fortalece la colaboración y la disciplina en equipos técnicos, y me dio confianza para futuros proyectos en equipos de desarrollo. Recomiendo, además, probar comandos adicionales y analizar la historia de commits para comprender el flujo completo del trabajo.
