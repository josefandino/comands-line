# PATH of FNM
readlink -f $(which node)

# Cuando se cambie la versión de NODE, se debe ejecutar lo siguiente:
sudo rm /usr/local/bin/node /usr/local/bin/npm
sudo ln -s $(readlink -f $(which node)) /usr/local/bin/node
sudo ln -s $(dirname $(readlink -f $(which node)))/npm /usr/local/bin/npm


