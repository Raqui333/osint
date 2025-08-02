
# 🐧 Introdução ao Linux e Comandos Essenciais

> 🗓️ Data: 02-08-2025

🏷️ **Tags**: #linux #terminal #comandos #shell #bash

---

## 📌 Resumo

O Linux é um sistema operacional amplamente utilizado em servidores, dispositivos embarcados e por desenvolvedores. Ele é baseado em Unix e oferece controle total do sistema por meio do terminal. Abaixo estão comandos fundamentais para navegar, manipular arquivos e controlar processos no Linux.

---

## Comandos Essenciais

- ### `ls`

  Lista o conteúdo de um diretório.  
  Exemplo:

  ```bash
  ls
  ls -l  # exibe em formato de lista
  ls -a  # mostra arquivos ocultos
  ```

- ### `cd`

  Muda o diretório atual.  
  Exemplo:

  ```bash
  cd /home/usuario
  cd ..  # volta um diretório
  cd ~   # vai para o diretório home
  ```

- ### `pwd`

  Mostra o caminho (path) do diretório atual.  
  Exemplo:

  ```bash
  pwd
  ```

- ### `find`

  Procura arquivos e diretórios.  
  Exemplo:

  ```bash
  find . -name arquivo.txt
  find /etc -type f -name "*.conf"
  ```

- ### `cat`

  Exibe o conteúdo de arquivos.  
  Exemplo:

  ```bash
  cat arquivo.txt
  ```

- ### `echo`

  Imprime uma mensagem na tela ou escreve em arquivos.  
  Exemplo:

  ```bash

  echo "Olá, Linux!"
  echo "Linha 1" > arquivo.txt     # sobrescreve o arquivo
  echo "Linha 2" >> arquivo.txt    # adiciona ao final do arquivo
  ```

---

## Operadores no Shell

- ### `&`

  Executa o comando em segundo plano.  
  Exemplo:

  ```bash
  ./script.sh &
  ```

- ### `&&`

  Executa o segundo comando somente se o primeiro tiver sucesso.  
  Exemplo:

  ```bash
  mkdir pasta && cd pasta
  ```

- ### `>`

  Redireciona a saída (stdout) para um arquivo, **sobrescrevendo** o conteúdo.  
  Exemplo:

  ```bash
  echo "Hello" > output.txt
  ```

- ### `>>`

  Redireciona a saída (stdout) para um arquivo, **adicionando** ao final.  
  Exemplo:

  ```bash
  echo "World" >> output.txt
  ```
