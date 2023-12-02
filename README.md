# zyte-tutorial

https://www.python.org/downloads/windows/
Download Windows x86-64 executable installer

version de python 3.8 o superior (pero menor a 3.10, la 3.12 da error)

# PASOS

python --version
mkdir web-scraping-tutorial
cd web-scraping-tutorial

python -m venv tutorial-env
cd .\tutorial-env\
ls
cd ..
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope Process

cd .\Scripts\
.\activate
cd ..
pip install --upgrade 'scrapy>=2.11'
cd ..
scrapy startproject tutorial .

(creamos la carpeta en la raiz, fuera de la carpeta tutorial-env)
(tutorial-env) PS C:\Users\crist\OneDrive\Escritorio\web-scraping-tutorial> scrapy startproject tutorial .

probar archivo python: python .\demo.py

para salir del entorno virtual: exit

web de pruebas para web-scraping:
http://books.toscrape.com/

(tutorial-env) PS C:\Users\crist\OneDrive\Escritorio\web-scraping-tutorial> pip install --upgrade shub

Cree un archivo de texto vacío en web-scraping-tutorial/requirements.txt y añadir esto : scrapy==2.5.1

Cree un archivo YAML en web-scraping-tutorial/scrapinghub.yml

requirements:
file: requirements.txt
stacks:
default: scrapy:2.11

shub login
API KEY

shub deploy 728780

para salir -> shub logout
