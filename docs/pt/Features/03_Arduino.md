# Flash

Você pode habilitar auto-flashing com `--flash`.

Para fazer isso, você precisa do avrdude.

## Instalando o avrdude

No Debian ou Ubuntu, apenas use :

```
sudo apt-get update && sudo apt-get install avrdude
```

No Windows, faça o download e instale a ultima versão da IDE do Arduino : https://www.arduino.cc/en/Main/Software

## Usando --flash

A opção `--flash` requer a porta COM.

Exemplo do Windows, com cabo USB plugado em um Arduino Mega 2560 :

```
nectar --target arduino-mega2560 --flash COM0 arduino.js
```

Exemplo do Debian, com cabo USB plugado em um Arduino Mega 2560 :

```
nectar --target arduino-mega2560 --flash /dev/ttyACM0 arduino.js
```

Você pode obter mais informações usando `--verbose`
