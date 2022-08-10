
# Ruby en WSL

Instalación de Ruby on Rails en Windows con WSL, en 4 pasos

⚠️ Nota: Windows te pedirá reiniciar. Es importante que no tengas nada importante abierto!

## Preparación


- 👉 [Toca aquí para descargar](https://codeload.github.com/sebacarrasco93/ruby-wsl/zip/refs/heads/main)

- Descomprime la descarga en tu PC con WinRar, WinZip o con el mismo explorador de Windows, y abre la nueva carpeta descomprimida llamada "ruby-wsl"

## Pasos en Windows

- Abre la carpeta "**windows**" y busca "**1.cmd**". Usa el click derecho sobre el archivo y haz click donde dice "**Ejecutar como administrador**"... 🤞 Paciencia, se va a demorar!

- Cuando termine, haz lo mismo con "**2.cmd**", y espera hasta que se abra Ubuntu

## Pasos en Ubuntu

💡 Tip: Cuando Ubuntu se abra por primera vez, te pedirá crear un usuario y contraseña, pueden ser distintos a los de Windows

---

Una vez listo, copia línea estas dos líneas (y después presiona `enter`)

```sh
git clone https://github.com/sebacarrasco93/ruby-wsl
sh ruby-wsl/ubuntu/1.sh
```

Después esta línea (y después, `enter` también)

```sh
sh ruby-wsl/ubuntu/2.sh
```

Listo! ✨

## Probando

Si salió todo bien, en Ubuntu deberías ser capaz de crear un proyecto de Ruby on Rails

```sh
rails new tu_proyecto -T
```

> No olvides cambiar `tu_proyecto` por un nombre tuyo

Después, deberías poder entrar a la carpeta

```sh
cd tu_proyecto
```

Deberías ser capaz de abrir el servidor puma (dentro de `tu_proyecto`)

```sh
puma
```

En Windows, abre la URL [http://127.0.0.1:3000](http://127.0.0.1:3000). Deberías poder ver el mensaje de bienvenida de Ruby on Rails

### Notas

Si tienes sugerencias o encuentras un error, hazme un fork y un push en GitHub.

Si te funcionó y te gustó, escríbeme a mi [Telegram](https://t.me/SebaCarrasco93), acepto cervezas heladitas 🍻!

### Referencias y recursos utilizados

- [GitBook](https://sickdata.gitbook.io/wsl/ruby) de Nicolás Bertín
