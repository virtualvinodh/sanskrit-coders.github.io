---
title: Testing
---

## Intro
- One can only test sequences in font+rendering engine combination.

### To test using the harfbuzz rendering engine:
Instructions [here](https://groups.google.com/d/msg/sanskrit-programmers/PEQBZ4b4OOg/pPlKqPeEI74J).

  -  hb-view /usr/share/fonts/truetype/ttf-devanagari-fonts/sahadeva.ttf
    अत्र

### pango

Supposedly can render with HarBuzz or Uniscribe or CoreText!

- pango-view --font "Sahadeva 40" -t अत्र
- pango-view --markup --text '\<span font\_family="FreeSerif"
lang="sa" fallback="false"\> अत्र\'

- Markup language
    [here](http://www.pygtk.org/pygtk2reference/pango-markup-language.html).

### Testing on Chrome

Fonts can also be tested on chrome by following a two step process.


- Install the font.
- Choose to use the font in Chrome:
  - Go to settings
  - Search for "font" in settings
  - get to the "Customize fonts" button
  - set all choices to the font you test. Or view a text file in Chrome after setting just the monospace font.
- gmail and its compose window may use some other
font.

### Other tools
- Google [font
tester](http://www.google.com/fonts#ChoosePlace:select/Script:devanagari).


## Text to test

  - [svara-s
    in](http://www.sanskritweb.net/sansdocs/tbsvaras.pdf)
    taittirIya-brAhmaNa.
  - [Rgveda
    scan](https://en.wikipedia.org/wiki/File:Rigveda_MS2097.jpg).

```
कॢप्तिः। ॐ॥ प्रीतिः। लोगों को देखो। हाँ। ಹಿಮಾದ್ರಿಸುತೇ ಪಾಹಿ ಮ್ಮಾಮ್।

धातुपाठे गमॢ। अश्वरुहः। शङ्करः।  काळी काळे।

Check udAtta and anudAtta collusions.
अ॒ग्निमी॑ळे पु॒रोहि॑तं य॒ज्ञस्य॑ दे॒वमृ॒त्विज॑म् । 
मू॒ मॄ॒ मॢ॒ मॣ॒। ई॑ ऐ॑ ओ॑ औ॑ अं॑ अ॑ः। मि॑ मी॑ मे॑ मै॑ मो॑ मौ॑ मं॑ 

Visarga and anusvAra with svara modifiers
म॑ं म॑ः
ससजुषो रुँः ।

Check anunAsika ँ collision
अनुनासिकचिह्नम् - लीँ

क्त्य क्त्व छ्य ड्य।

ೱ ೲ ᳵ ᳶ
लीँ

कॆ कॊ कॅ
```


## Report bugs

[GNU Freefont](https://savannah.gnu.org/bugs/?group=freefont).
Chrome.
  - Outstanding bugs: . (Reported bugs:
    [here](https://code.google.com/p/chromium/issues/list?can=1&q=vishvas&colspec=ID+Pri+M+Week+ReleaseBlock+Cr+Status+Owner+Summary+OS+Modified&x=m&y=releaseblock&cells=tiles).)
Free desktop
  - Outstanding bugs
    [1](https://bugs.freedesktop.org/show_bug.cgi?id=70509).
Noto \[[here](https://github.com/googlei18n/noto-fonts/issues)\]
