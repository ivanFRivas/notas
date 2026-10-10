




Buenas prácticas para montar Box
1. Desmontar correctamente (cuando quieras cerrarlo):

fusermount -u ~/box-diagramas

2. Montaje recomendado (con caché y logs):

rclone mount box:diagramas ~/box-diagramas \
  --daemon \
  --vfs-cache-mode writes \
  --dir-cache-time 5m \
  --poll-interval 1m \
  --log-file ~/rclone-box.log \
  --log-level INFO


3. Ver si está montado:

findmnt ~/box-diagramas
# o
mount | grep rclone


4. Si alguna vez el directorio queda “sucio” (archivos fantasma o error de montaje):

fusermount -u ~/box-diagramas
# Si falla:
sudo umount -l ~/box-diagramas



5. Resumen rápido de uso diario

# Montar
rclone mount box:diagramas ~/box-diagramas --daemon --vfs-cache-mode writes

# Usar normalmente (copiar, editar, etc.)
ls ~/box-diagramas
# ...

# Desmontar al terminar
fusermount -u ~/box-diagramas



