- Instala los portales de escritorio XDG: `sudo pacman -S xdg-desktop-portal xdg-desktop-portal-gtk`

- Habilitar el selector de archivos en Firefox. Abrir Firefox y escribir `about:config` en la barra de direcciones. Aceptar la advertencia de riesgo. Buscar la preferencia: `widget.use-xdg-desktop-portal.file-picker`. Hacer doble clic sobre ella para cambiar su valor a 1 (si está en false, cámbiarlo a true). Reiniciar Firefox.

- Asignar el gestor de archivos (GUI, NO CLI) (Caja, Thunar) por defecto. Mediante el comando en terminal `xdg-mime default **caja**.desktop inode/directory` crear el archivo de configuración.

- Asegurarse de que D-Bus esté correctamente iniciado junto a la sesión de DWM en el archivo .xinitrc/.xprofile con la siguiente linea `exec dbus-launch --exit-with-session dwm` (y NO `exec dwm`)

- Cerrar firefox, y reiniciar el sistema
