# translateColumnExcel
Traduci l'intera colonna di un file excel.

 ## Requisiti e compatibiltà
 Lo script è stato scritto utilizzando Python3 e deve essere lanciato con questo. 
 Testato su windows 10 e linux
 
 I moduli che ho utilizzato per creare lo script sono i seguenti :
 
 * openpyxl
 * colorama
 * googletrans
 * progressbar

# Installazione su Windows 
**Se hai già installato python3 puoi pure saltare questo pezzo**

* Scaricare ed installare Python da qui (https://www.python.org/downloads/). L'ultima versione che vi propone va benissimo;
  **NB: durante l'installazione selezionare la casella *Add Python to PATH***;
  
* Riavviare il computer;
* Scaricare questo repository in formato zip cliccando sul bottone verde 'Clone or Download';
* Estrarre il file zip in una cartella;
* Eseguire il file `traduttore-colonna-from-excel-setup` per installare automaticamente i moduli di Python richiesti.
* Ora potete lanciare `traduttore-colonna-from-excel.bat`

Enjoy :)

# Installazione su Linux  

```bash
git clone https://github.com/0v3rFlow/translateColumnExcel.git
cd translateColumnExcel
pip install -r requirements.txt
```

Enjoy :)

# Utilizzo

## Premessa
 Il file excel deve essere in formato xlsx e deve avere solamente la prima colonna del file (colonna A) valorizzata.

1 ) Inserite il nome del file excel se lo avete all'interno della cartella dello script(consiglio), oppure inserite il percorso del file.

```bash
Traduci la prima colonna del file excel da 'it' a xx. Verrà utilizzato Google Translate
[FILE] #Inserisci il percorso del file o il nome, se si trova nella stessa directory dello script 
```

2 ) Inserite la lingua per la quale si vuole tradurre la colonna. 

```bash
[XX]   #Inserisci il codice della lingua. 
```
3 ) Lo script andrà a prendere il foglio attivo e andrà a leggere riga per riga tutte le parole/frasi contenute nella prima colonna (colonna A) andando a scrivere la traduzione nella colonna successiva (colonna B)

  **NB: inserire il codice che identifica la lingua itilizzato da google traduttore. ES: it/en/ ecc.. In basso troverai le lingue supportate. ***; 
  
```bash
  LANGUAGES = {
    'af': 'afrikaans',
    'sq': 'albanian',
    'am': 'amharic',
    'ar': 'arabic',
    'hy': 'armenian',
    'az': 'azerbaijani',
    'eu': 'basque',
    'be': 'belarusian',
    'bn': 'bengali',
    'bs': 'bosnian',
    'bg': 'bulgarian',
    'ca': 'catalan',
    'ceb': 'cebuano',
    'ny': 'chichewa',
    'zh-cn': 'chinese (simplified)',
    'zh-tw': 'chinese (traditional)',
    'co': 'corsican',
    'hr': 'croatian',
    'cs': 'czech',
    'da': 'danish',
    'nl': 'dutch',
    'en': 'english',
    'eo': 'esperanto',
    'et': 'estonian',
    'tl': 'filipino',
    'fi': 'finnish',
    'fr': 'french',
    'fy': 'frisian',
    'gl': 'galician',
    'ka': 'georgian',
    'de': 'german',
    'el': 'greek',
    'gu': 'gujarati',
    'ht': 'haitian creole',
    'ha': 'hausa',
    'haw': 'hawaiian',
    'iw': 'hebrew',
    'hi': 'hindi',
    'hmn': 'hmong',
    'hu': 'hungarian',
    'is': 'icelandic',
    'ig': 'igbo',
    'id': 'indonesian',
    'ga': 'irish',
    'it': 'italian',
    'ja': 'japanese',
    'jw': 'javanese',
    'kn': 'kannada',
    'kk': 'kazakh',
    'km': 'khmer',
    'ko': 'korean',
    'ku': 'kurdish (kurmanji)',
    'ky': 'kyrgyz',
    'lo': 'lao',
    'la': 'latin',
    'lv': 'latvian',
    'lt': 'lithuanian',
    'lb': 'luxembourgish',
    'mk': 'macedonian',
    'mg': 'malagasy',
    'ms': 'malay',
    'ml': 'malayalam',
    'mt': 'maltese',
    'mi': 'maori',
    'mr': 'marathi',
    'mn': 'mongolian',
    'my': 'myanmar (burmese)',
    'ne': 'nepali',
    'no': 'norwegian',
    'ps': 'pashto',
    'fa': 'persian',
    'pl': 'polish',
    'pt': 'portuguese',
    'pa': 'punjabi',
    'ro': 'romanian',
    'ru': 'russian',
    'sm': 'samoan',
    'gd': 'scots gaelic',
    'sr': 'serbian',
    'st': 'sesotho',
    'sn': 'shona',
    'sd': 'sindhi',
    'si': 'sinhala',
    'sk': 'slovak',
    'sl': 'slovenian',
    'so': 'somali',
    'es': 'spanish',
    'su': 'sundanese',
    'sw': 'swahili',
    'sv': 'swedish',
    'tg': 'tajik',
    'ta': 'tamil',
    'te': 'telugu',
    'th': 'thai',
    'tr': 'turkish',
    'uk': 'ukrainian',
    'ur': 'urdu',
    'uz': 'uzbek',
    'vi': 'vietnamese',
    'cy': 'welsh',
    'xh': 'xhosa',
    'yi': 'yiddish',
    'yo': 'yoruba',
    'zu': 'zulu',
    'fil': 'Filipino',
    'he': 'Hebrew'
}
```

# FINE!
