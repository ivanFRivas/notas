#nb

# si el directorio está vacío o no existe:
git clone git@github.com:ivanFRivas/notas.git /home/ivan/Notas

# si ya existe pero vacío:
cd /home/ivan/Notas
git init
git remote add origin git@github.com:ivanFRivas/notas.git
git fetch origin
git checkout -t origin/main   # o master, según tu rama


# al parecer, al ejecutar nb, este busca en la carpeta desde donde esta la terminal.
