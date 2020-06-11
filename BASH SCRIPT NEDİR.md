# BASH SCRIPT NEDİR ? 

## BASH SCRIPT 

Dilerseniz "*Script nedir?*' ve '*Bash Script Nedir?*'' sorularını uzun bir şekilde anlatmak yerine örneklerle bunu açıklama yoluna gidelim. Linux işletim sisteminizde .sh uzantılı bir dosya açarak scriptinizi bu dosyaya yapıştıralım. 

```bash
#!/bin/bash
# Basit bir script
# GOKAYBURUC 10/6/2020
 
echo Klasörün içeriği aşağıda yer almaktadır:
ls -l
```



Bu scripti terminalde aşağıdaki gibi çalıştırırsanız.

```bash
$ sh myscript.sh 
```

**Çıktı (Output)**:

```bash
Here are the files in your current directory:
total 72
-rw-rw-r-- 1 gokayburuc gokayburuc 3605 Haz  9 14:00 anki_line_sentences.csv
-rw-rw-r-- 1 gokayburuc gokayburuc 2579 Haz  9 13:42 anki_sentences.csv
-rw-rw-r-- 1 gokayburuc gokayburuc 1223 Haz  9 13:40 article.txt
-rw-rw-r-- 1 gokayburuc gokayburuc 2105 Haz  9 11:50 article_wordlist.csv
-rw-rw-r-- 1 gokayburuc gokayburuc  583 Haz  9 10:53 google_trans_text.py
```



Şimdi ikinci bir script yazalım. 

```bash
#!/bin/bash
# mp3 dosyalarini otomatik olarak bir klasöre toplayan script
mkdir MP3_FILES/
mv *.mp3 MP3_FILES/
```

Bu script ise mp3 dosyalarınızı bir klasöre toplamayı sağlar.

**Çıktı (Output)**:

```bash
~/Music$ ls 
MP3_FILES  mp3_script.sh
```

Artık bu scripti çalıştırdığımız klasörde mp3 uzantılı dosyaları MP3_FILES isimli bir klasör oluşturup bu verileri içeriye dolduracaktır. 