# Verificar a sintaxe

Você pode apenas verificar a sintaxe sem compilação com argumento `--check`.

# Gerenciamento do projeto

Se `--single` não for especificado, NectarJS irá criar um arquivo `project.json` no diretorio do projeto.

Você pode criar um arquivo `project.json` sem compilação com : `nectar --prepare file.js`

Para exibir a configuração do projeto : `nectar --project` na pasta do projeto ou `nectar --project /path/to/projet.json`

Para compilar o projeto, simplesmente use `nectar project.json`

# Dicas

Você pode habilitar dicas usando `--tips`.

Exemplo :

```
nectar --target arduino-uno --tips arduino.js
```

Isso irá exibir :

```
[*] Tips : avrdude -p ATMEGA328P -c arduino -P [COMPORT] -b 19200 -F -U flash:w:arduino-arduino-uno.hex
```
