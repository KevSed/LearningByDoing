#ArchLinux

##[Default Applications](https://wiki.archlinux.org/index.php/Default_applications)
Arch uses the command xdg-open to open URL/Files/... with its standard Type.
For this it calls the default application fiven by its [MIME Type](https://en.wikipedia.org/wiki/Media_type). E.g. for https://www.google.de this is x-scheme-handler/https.
To change the default application for a https mime time use following command:
```
xdg-mime default firefox.desktop x-scheme-handler/https
```
This redirects the command:
```
xdg-open https://www.google.de
```
to /usr/share/applications/firefox.desktop
### Change standard Browser in Jupyter Notebook:
* Generate config 
```
jupyter notebook --generate-config
vim ~/.jupyter/jupyter_notebook_config.py
```
* Change #c.NotebookApp.browser = '' to c.NotebookApp.browser = 'xdg-open'
