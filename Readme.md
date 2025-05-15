# PuTTY Color Themes
Queto elenco di file permette di personalizzare i colori della Putty su Windows modificando le impostazioni del registro di sistema.
Per ogni sessione che viene creata nella Putty, viene salvata una voce nel registro di sistema sotto la chiave
`Computer\HKEY_CURRENT_USER\SOFTWARE\SimonTatham\PuTTY\Sessions\Nome%20Sessione`
con tutte le impostazioni che salviamo nella nostra sessione.

## Come utilizzare questi file
1. Dall'elenco delle immagini, selezioniamo lo schema colore che piu ci aggrada (comprende un po tutti i parametri colore) [here](images/readme.md)
2. Quindi scarichiamo il file che ci interessa ed apriamolo in modifica, andando a modificare il nome della sessione all'interno della posizione della chiave
    `Computer\HKEY_CURRENT_USER\SOFTWARE\SimonTatham\PuTTY\Sessions\Nome%20Sessione` -> `Computer\HKEY_CURRENT_USER\SOFTWARE\SimonTatham\PuTTY\Sessions\Nome%20Personalizzato%20Sessione` 
3. Una volta salvato, eseguiamo un doppio click sul file ed autorizziamo windows alla modifica del file di registro.
4. Nel programma è specificato di poter eseguire il D&D del file _.reg_ sul file _.js_ presente nel repository. Questa funzione non viene eseguita ma non è necessaria se facciamo come indicato sopra
    Drag'n'Drop reg-file on `_puttycolor.js` in Windows Explorer for applying theme on saved PuTTY sessions
5. Enjoy it!

## La struttura del file di registro
```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\SimonTatham\PuTTY\Sessions\SESSION_NAME]

; Default Foreground
"Colour0"="217,216,216"
; Default Bold Foreground
"Colour1"="217,216,216"
; Default Background
"Colour2"="28,28,28"
; Default Background
"Colour3"="28,63,149"
; Cursor Text
"Colour4"="28,28,28"
; Cursor Color
"Colour5"="231,231,232"
; ANSI Black
"Colour6"="115,113,113"
; ANSI Black Bold
"Colour7"="115,113,113"
; ANSI Red
"Colour8"="251,38,8"
; ANSI Red Bold
"Colour9"="251,38,8"
; ANSI Green
"Colour10"="167,226,46"
; ANSI Green Bold
"Colour11"="167,226,46"
; ANSI Yellow
"Colour12"="102,217,238"
; ANSI Yellow Bold
"Colour13"="102,217,238"
; ANSI Blue
"Colour14"="0,157,220"
; ANSI Blue Bold
"Colour15"="0,157,220"
; ANSI Magenta
"Colour16"="255,85,255"
; ANSI Magenta Bold
"Colour17"="255,85,255"
; ANSI Cyan
"Colour18"="255,210,4"
; ANSI Cyan Bold
"Colour19"="255,210,4"
; ANSI White
"Colour20"="217,216,216"
; ANSI White Bold
"Colour21"="255,255,255"
```
----
Original [putty.org.ru](http://putty.org.ru/themes/index.html)
Now avaliable on [webarchive]( https://web.archive.org/web/20151122030926/http://putty.org.ru:80/themes/index.html)
Disponibile anche [DareKay](https://darekkay.com/blog/my-putty-color-scheme/)
