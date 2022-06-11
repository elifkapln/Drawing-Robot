# Drawing-Robot

Neyi Amaçlar?

Tasarlanan VM (Virtual Machine), seçilen herhangi bir .txt uzantılı dosyayı okuyarak içerisinde
bulunan komutlara göre çizgi çizer. (Örnek bir dosya: [example.txt](https://github.com/elifkapln/Drawing-Robot/files/8884803/example_txt.txt) )


Nasıl Kullanılır?

- Program çalıştırıldıktan sonra **Choose File** butonuna tıklanarak komutların okunacağı .txt uzantılı dosya seçilir.
- Seçilen dosyanın içerdiği komutlar _mavi panelde_ gösterilir. 
- Komutlarda bir _'syntax'_ hatası bulunmuyorsa, _beyaz panele_ çizim yapılır. 
- Eğer komutlarda bir hata tespit edildiyse, hata mesajı _yeşil panelde_ gösterilir.

Nasıl Çalışır?

Çizgi Çizen VM, okuduğu her dosyanın içinde bulunan komutların **'lexical analysis'**
işlemini yapar, daha önce gramerler ile belirlenmiş 'syntax' kurallarına göre **'parsing'** işlemini
yapar. Bu aşamada bir hata ile karşılaşılırsa, hata mesajı yeşil panelde gösterilir. Eğer dosyadan
alınan komutlar hatasız ise çizim yapılır.

Çalıştırmak İçin Neler Gerekli?

Bu program, _VS Code_ platformunda, _Python_ diline ait Turtle, Tkinter ve PLY (LEX/YACC) ile
programlanmıştır. **lex.py** ve **yacc.py** dosyaları, programı çalıştırmak için gerekli ve yeterlidir.
