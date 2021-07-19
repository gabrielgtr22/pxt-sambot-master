
# sambot Package
This Samdu sambot package was developed by [SamEdu](https://samedu.com.br/).

The SamEdu sambot is a small educational robot by the BBC micro:bit. The Sambot extends the micro:bit's 3 GPIO ports and allow for different sensors and components to be easily attached to the micro:bit. A basic sambot can be easily programmed to run autonomously, with a remote control, and even create rainbow beacons of light. Just add one of the many extensions available and your sambot can do even more things like line and light following, obstacle avoiding, drawing and more! 

![](https://i.imgur.com/lCXh03y.png)



## Code Example
```JavaScript

let strip: neopixel.Strip = null
sambot.init_wheel(AnalogPin.P1, AnalogPin.P2)
strip = neopixel.create(DigitalPin.P0, 24, NeoPixelMode.RGB)
strip.showRainbow(1, 360)
basic.showIcon(IconNames.Heart)
basic.forever(function () {
    strip.rotate(1)
    basic.pause(100)
    strip.show()
})
basic.forever(function () {
    sambot.freestyle(30, 90)
    basic.pause(1500)
    sambot.freestyle(90, 30)
    basic.pause(1500)
})


```

## License
MIT

## Supported targets
for PXT/microbit (The metadata above is needed for package search.)




> Abrir essa página em [https://gabrielgtr22.github.io/pxt-sambot-master/](https://gabrielgtr22.github.io/pxt-sambot-master/)

## Usar como extensão

Este repositório pode ser adicionado como **extensão** no MakeCode.

* abrir [https://makecode.microbit.org/](https://makecode.microbit.org/)
* clique em **Novo Projeto**
* clique em **Extensões** em baixo do menu com ícone de engrenagem
* procure por **https://github.com/gabrielgtr22/pxt-sambot-master** e importe

## Editar este projeto ![Ícone de estado da compilação](https://github.com/gabrielgtr22/pxt-sambot-master/workflows/MakeCode/badge.svg)

Para editar este repositório no MakeCode.

* abrir [https://makecode.microbit.org/](https://makecode.microbit.org/)
* clique em **Importar** e depois clique em **Importar URL**
* cole **https://github.com/gabrielgtr22/pxt-sambot-master** e clique em importar

## Pré-visualização de blocos

"Essa imagem mostra o bloco de códigos da última confirmação no "mestre"".
Esta imagem pode demorar alguns minutos para atualizar.

![Uma visão renderizada dos blocos](https://github.com/gabrielgtr22/pxt-sambot-master/raw/master/.github/makecode/blocks.png)

#### Metadados (usados para pesquisa, renderização)

* for PXT/microbit
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
