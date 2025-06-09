=== INSTRUCCIONES DE INSTALACIÓN ===

Para instalar correctamente la PWA, siga estos pasos:

1. Cree la siguiente estructura de carpetas:
   /
   ├── index.html           (en la raíz)
   ├── service-worker.js    (en la raíz)
   ├── manifest.json        (en la raíz)
   ├── favicon.ico          (en la raíz)
   └── icons/
       ├── icon-192.png
       └── icon-512.png

2. Coloque los archivos en el lugar correcto:
   - Todos los archivos HTML, JS y JSON deben ir en la raíz
   - favicon.ico debe ir en la raíz
   - Las imágenes (icon-192.png y icon-512.png) deben ir en la carpeta "icons"

3. Suba todos los archivos a su servidor web

4. Asegúrese de que su servidor web:
   - Sirve los archivos con los tipos MIME correctos
   - Tiene HTTPS habilitado (requerido para PWAs)

5. Visite su sitio web desde un dispositivo móvil y debería ver el banner de instalación

=== NOTAS IMPORTANTES ===

- Las PWAs requieren HTTPS para funcionar correctamente
- Pruebe su PWA en diferentes navegadores y dispositivos
- El banner de instalación solo aparecerá si se cumplen los criterios del navegador
- Para forzar la actualización de la caché, cambie la versión en service-worker.js

=== SOLUCIÓN DE PROBLEMAS ===

Si su PWA no se instala correctamente:
- Verifique que todos los archivos estén en las ubicaciones correctas
- Compruebe que su servidor esté configurado para HTTPS
- Utilice Chrome DevTools > Application > Manifest para depurar problemas
- Verifique que el service worker esté registrado correctamente en Chrome DevTools > Application > Service Workers
