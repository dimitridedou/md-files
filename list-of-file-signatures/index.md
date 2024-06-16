**Offiset** : Mια μετατόπιση εντός ενός πίνακα ή άλλου αντικειμένου δομής δεδομένων είναι ένας ακέραιος αριθμός που υποδεικνύει την απόσταση (μετατόπιση) μεταξύ της αρχής του αντικειμένου και ενός δεδομένου στοιχείου ή σημείου, πιθανώς εντός του ίδιου αντικειμένου.Η έννοια της απόστασης ισχύει μόνο εάν όλα τα στοιχεία του αντικειμένου έχουν το ίδιο μέγεθος (συνήθως δίνονται σε byte ή λέξεις).

Για παράδειγμα, εάν το A είναι ένας πίνακας χαρακτήρων που περιέχει "abcdef", το τέταρτο στοιχείο που περιέχει τον χαρακτήρα "d" έχει μετατόπιση 3 από την αρχή του A.


# Document

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
| `25 50 44 46 2D`| `%PDF-` |0|pdf|Portable Document Format|


# Video

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
|`52 49 46 46 ?? ?? ?? ??` <br> `57 41 56`|`RIFF????AVI␠`|0|avi|Audio Video Interleave video format|
|`66 74 79 70 69 73 6F 6D`|`ftypisom`|4|mp4|ISO Base Media file (MPEG-4)|


# Αρχεία Ηχου

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
| `FF FB`   `FF F3`   `FF F2` |`ÿû` `ÿó` `ÿò`|0|mp3	 | MPEG-1 Layer 3 file without an ID3 tag or with an ID3v1 tag (which is appended at the end of the file)|
|`49 44 33`	|`ID3`|0|mp3|MP3 file with an ID3v2 container|
|`52 49 46 46 ?? ?? ?? ??` <br> `57 41 56 45` |`RIFF????WAVE`|0|wav|Waveform Audio File Format|



# Αρχεία Εικόνας

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
| `89 50 4E 47 0D 0A 1A 0A`	|`‰PNG␍␊␚␊`| 0|png |  |
|`47 49 46 38 37 61`|`GIF87a`|0|gif	|Image file encoded in the Graphics Interchange Format (GIF)|
|`47 49 46 38 39 61 `|`GIF89a`|0|gif|Image file encoded in the Graphics Interchange Format (GIF)|
|`49 49 2A 00`|`II*␀`|0|tif|(little-endian) Tagged Image File Format|
|`4D 4D 00 2A`|`MM␀*`|0|tiff|(big-endian) Tagged Image File Format|
|`38 42 50 53`|`8BPS`|0|psd|Photoshop Document file, Adobe Photoshop's native file format|


# Compressed Archiver - compressed file

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
|`52 61 72 21 1A 07 00`	|`Rar!␚␇␀`|0| rar | Roshal ARchive compressed archive v1.50 onwards|
|`52 61 72 21 1A 07 01 00`	|`Rar!␚␇␁␀`|0|rar|Roshal ARchive compressed archive v5.00 onwards|
|`1F 9D`|`␟□`|0| z' tar.z|compressed file (often tar zip) using Lempel-Ziv-Welch algorithm|
|`1F A0`|`␟⍽`|0| z tar.z|Compressed file (often tar zip) using LZH algorithm|
|'37 7A BC AF 27 1C`|`7z¼¯'␜`|0|7z|7-Zip File Format|
|`1F 8B`|`␟‹`|0|gz   tar.gz|GZIP compressed file|

> zip file format and formats based on it, such as EPUB, JAR, ODF, OOXML

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
|`50 4B 03 04`|`PK␃␄`|0|zip    aar   apk   docx   epub   ipa   jar   kmz    maff   msix   odp   ods   odt   pk3   pk4   pptx   usdz   vsdx   xlsx   xpi|zip file format and formats based on it, such as EPUB, JAR, ODF, OOXML|
|`50 4B 07 08`   (spanned archive)|`PK␃␄`|0|zip    aar   apk   docx   epub   ipa   jar   kmz    maff   msix   odp   ods   odt   pk3   pk4   pptx   usdz   vsdx   xlsx   xpi|zip file format and formats based on it, such as EPUB, JAR, ODF, OOXML|
|`50 4B 05 06`   (empty archive)|`PK␃␄`|0|zip    aar   apk   docx   epub   ipa   jar   kmz    maff   msix   odp   ods   odt   pk3   pk4   pptx   usdz   vsdx   xlsx |xpi zip file format and formats based on it, such as EPUB, JAR, ODF, OOXML|


# Lunix

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
|`21 3C 61 72 63 68 3E 0A`|`!<arch>␊`|0|deb|linux deb file|

# SQL

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
|`53 51 4C 69 74 65 20 66`  `6F 72 6D 61 74 20 33 00` |`SQLite format 3␀`|0|sqlitedb   sqlite   db  | SQLite Database|


# Executable

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
|`4D 5A`	|`MZ`|0|exe   scr   sys   dll   fon   cpl   iec   ime   rs    tsp   mz | DOS MZ executable and its descendants (including NE and PE)|
|`7F 45 4C 46`	| |0| | Executable and Linkable Format|



# Διαφορά

| Hex signature |ISO 8859-1 |Offset|Επέκταση|Περιγραφή|
|----------|:-:|:-:|-|-|
| `43 44 30 30 31`|`CD001`|`0x8001` `0x8801` `0x9001` |iso | ISO9660 CD/DVD image file |
| `53 50 30 31`	|`SP01`|0|bin |Amazon Kindle Update Package|
