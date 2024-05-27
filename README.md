![](https://komarev.com/ghpvc/?username=iuricode&color=006bed)

## Sobre mim

- 🤔 Explorando novas tecnologias.
- 🎓 Estudando 
- 🌱 Aprendendo mais sobre {desenvolvimento de sistemas}.


![C++](https://img.shields.io/badge/-C++-333333?style=flat&logo=C%2B%2B&logoColor=00599C)
![Java](https://img.shields.io/badge/-Java-333333?style=flat&logo=Java&logoColor=007396)
![JavaScript](https://img.shields.io/badge/-JavaScript-333333?style=flat&logo=javascript)

name: Deploy Animation

on:
  push:
    branches: [ main ]

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v3

      - name: Build Project
        run: # Replace with your build commands

      - name: Deploy Animation
        uses: actions/upload-artifact@v3
        with:
          name: animation
          path: ./animation.svg
          retention-days: 10

