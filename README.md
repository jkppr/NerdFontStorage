# Nerd Font for Terminal on chromeOS
Storing some Nerd Fonts to be used with Crostini (Linux on Chrome OS)

To get `powerlevel10k` working with my chromeOS crostini I followed the instructions here: https://github.com/romkatv/powerlevel10k#meslo-nerd-font-patched-for-powerlevel10k
 (last entry in step 3).

 However, I want to have control over the loaded fonts myself so I host them in this repository.

TL;DR:

1. Open `chrome-untrusted://terminal/html/nassh_preferences_editor.html` in chrome. 
2. Add `'MesloLGS NF'` to Text font family 
3. Add the css below to Custom CSS (inline text):

```
@font-face {
 font-family: "MesloLGS NF";
 src: url("https://raw.githubusercontent.com/jkppr/NerdFontStorage/master/MesloLGS_fonts/MesloLGS%20NF%20Regular.ttf");
 font-weight: normal;
 font-style: normal;
}
@font-face {
    font-family: "MesloLGS NF";
    src: url("https://raw.githubusercontent.com/jkppr/NerdFontStorage/master/MesloLGS_fonts/MesloLGS%20NF%20Bold.ttf");
    font-weight: bold;
    font-style: normal;
}
@font-face {
    font-family: "MesloLGS NF";
    src: url("https://raw.githubusercontent.com/jkppr/NerdFontStorage/master/MesloLGS_fonts/MesloLGS%20NF%20Italic.ttf");
    font-weight: normal;
    font-style: italic;
}
@font-face {
    font-family: "MesloLGS NF";
    src: url("https://raw.githubusercontent.com/jkppr/NerdFontStorage/master/MesloLGS_fonts/MesloLGS%20NF%20Bold%20Italic.ttf");
    font-weight: bold;
    font-style: italic;
}
```
