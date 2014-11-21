class: center, middle, inverse
# Haxe - The Cross-platform Toolkit
## meetup Web Dev des Savoie - 11/2014
---

class: center, middle
# ![haxe logo](haxe-logo.svg)
### Créé en Octobre 2005, par Nicolas Cannasse en OCaml
### Haxe 2 en 2006
### Haxe 3 en 2012

.footnote[[->Wikipedia](https://en.wikipedia.org/wiki/Haxe)]
---

class: center, middle, inverse
# Toolkit
---

.left-column[
## Toolkit
### - Haxe language
]

.right-column[
### Proche d'ECMAScript / Java / C# / AS3
```haxe
class HelloWorld {
    static public function main() {
        trace("Hello World");
    }
}
```
```haxe
var point = { x: 0, y: 10 };
point.x += 10;
```
```haxe
for (i in 1...3) {
    trace(i);
}
```
```haxe
using StringTools;
"  Me & You    ".trim().htmlEscape();
```

.footnote[[-> Haxe Language Features](http://haxe.org/documentation/introduction/language-features.html)]
]
---

.left-column[
## Toolkit
### - Haxe language
### - Haxe standard library
]

.right-column[
### Top-level: `Array`, `Date`, `Lambda`, `Map`, `Math`, `String`,...
### Haxe package: `haxe.Json`, `haxe.Http`, `haxe.crypto`, `haxe.macro`, `haxe.unit`, `haxe.rtti`,...
### Data structure: `haxe.ds.ArraySort`, `haxe.ds.ObjectMap`, `haxe.ds.Vector`,...
### IO: `haxe.io.Bytes`, `haxe.io.BytesBuffer`, `haxe.io.Path`
### System API: `Sys.db`, `Sys.io.File`,...

.footnote[[-> Introduction to the Haxe Standard Library](http://haxe.org/documentation/introduction/stdlib-introduction.html)]
]
---

.left-column[
## Toolkit
### - Haxe language
### - Haxe standard library
### - Haxe compiler
]

.right-column[
## Haxe __Cross__-compiler
- Flash
- Neko
- JS
- AS3
- PHP
- C++
- Java
- C#
- Python
.footnote[[-> Compiler Targets](http://haxe.org/documentation/introduction/compiler-targets.html)]
]

???
---

.left-column[
## Toolkit
### - Haxe language
### - Haxe standard library
### - Haxe compiler
### - Haxelib
]

.right-column[
### Library manager
```json
{
  "name": "useless_lib",
  "url" :
      "https://github.com/jasononeil/useless/",
  "license": "MIT",
  "tags": ["cross", "useless"],
  "description":
      "This library is useless in the same way on
        every platform",
  "version": "1.0.0",
  "releasenote":
      "Initial release, everything is working
        correctly",
  "contributors": ["Juraj","Jason","Nicolas"],
  "dependencies": {
    "tink_macros": "",
    "nme": "3.5.5"
  }
}
```
```shell
haxelib search <library>
haxelib install <library>
haxelib update <library>
```
.footnote[[-> lib.haxe.org](http://lib.haxe.org/)]
]

???

---

class: center, middle, inverse
# Cross-platform
---

.left-column[
## Cross-platform
### - Games
]

.right-column[
  ## OpenFl
  [-> Showcase](http://www.openfl.org/showcase/)
  ## Flambe
  2D game engine, Haxe -> HTML5/Flash
  ### Evoland
  [LD#24](http://evoland.shirogames.com/classic)
]

???

---

.left-column[
## Cross-platform
### - Games
### - Web
]

.right-column[
  ## client
  Flash /SWF

  Haxe + Angular: [-> Haxejs.com](http://haxejs.com)
  ### Example
  [netwars](http://netwars-project.com/webdoc), [Prezi](http://prezi.com)
  ## server
  PHP, Neko,...

  Nodejs: [JS toolkit for Haxe](https://github.com/clemos/haxe-js-kit)

  .footnote[_Haxe, what JS should have been_]
]

???

---

.left-column[
## Cross-platform
### - Games
### - Web
### - Mobile
]

.right-column[
## OpenFl
OpenGL + C++ = win
## NME
ancêtre de OpenFL, fabriqué par Hugh Anderson, créateur de hxcpp, waxe,...
[website](http://nmehost.com/)
## Croxit
Cordova avec du haxe
]

???
---

.left-column[
## Cross-platform
### - Games
### - Web
### - Mobile
### - Desktop
]

.right-column[
## OpenFl
OpenGL + C++ = win (x2!)
## Waxe
WxWidgets
## Node webkit
]

???

---

class: center, middle, inverse
# [try.Haxe.org](http://try.haxe.org/)
