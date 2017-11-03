# chars.ahk

## Intro

`Chars.ahk` is a simple [AutoHotkey](https://www.autohotkey.com/) script that turns named character references (like `&eacute;`, `&pound;` or `&star;`) into actual accented characters, symbols, etc. (like `é`, `£` or `☆`), all on the fly. It's a workaround for Windows 10's poor character input support, which otherwise involves typing ALT codes or picking them from Character Map.

## Usage

1. Install [AutoHotkey](https://www.autohotkey.com/).
2. Download `chars.ahk` and double click it to run.
3. Go to any document and type in a named character reference (e.g. try `&ntilde;` and you'll see `ñ` appear)

To have it run automatically on startup, add a shortcut to `chars.ahk` from `%appdata%\Microsoft\Windows\Start Menu\Programs\Startup`.

## Reference

I used the HTML5's spec [named character references](https://www.w3.org/TR/html5/syntax.html#named-character-references) as a starting point, removed the ones without `;` at the end (unsure why they're there to begin with), and commented out `&amp;`, `&quot;`, `&lt;` and `&gt;` as they're typically available on keyboards, and there might be good reasons why you'd want to escape them as such.
