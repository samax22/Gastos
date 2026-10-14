# Mis gastos (Android)

App de gastos diarios con calendario, total del mes y plan de ahorro.
La interfaz está en `app/src/main/assets/index.html`. Si la cambias y subes el cambio, GitHub vuelve a compilar el APK.

## Compilar
Cada vez que subes cambios a la rama `main`, la acción **Compilar APK** genera el archivo.
Descárgalo en la pestaña **Actions** → la ejecución más reciente → **Artifacts** → `MisGastos-APK`.

## Actualizar sin perder datos
- La app se firma siempre con `app/misgastos.keystore`. **No lo borres ni lo cambies**: si cambia la firma, Android obliga a desinstalar y se pierden los datos.
- Para cambiar la app basta con reemplazar `app/src/main/assets/index.html` y subirlo. El número de versión sube solo.
- Los datos viven en el celular, no en el APK: instalar encima del anterior los conserva.
