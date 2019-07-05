
# Git kullanımı - Github bağlantısı

## Git
<br/>

![git](https://git-scm.com/images/logos/downloads/Git-Icon-Black.png)

`$ git config --global user.name "Erencan Cabuk"`

**Email yaratma** <br/>
`$ git config --global user.email "erncncbk@gmail.com"`

**Yaratılanları gösterme**<br/>
`$ git config --global user.name`
`$ git config --global user.email`

**Dosya dizinine gitme**<br/>
`$ pwd`

**Dosya dizinindeki dosyaları listeleme**<br/>
`$ ls`

**Dosya Açma**<br/>
`$ mkdir Proje   `

**Gidilmek istenen dizin komutu için (cd= change directory)** <br/>
`$ cd Proje`

**Dosya içinde text file oluşturma** <br/>
`$ touch text.txt`

**Dosya içine *'git'* dosyaları yükleme** <br/>
`$ git init`

**Oluşan *'git'* projesini *'geçiş bölgesine'* ekleme** <br/>
`$ git add .`

***'Geçiş bölgesine'* eklenen projeyi *'commit'* edip versiyon ismi verme**  <br/>
`$ git commit -m "versiyon1"`

**Oluşturulan modelleri ve versiyonları gösterme**<br/>
`$ git log`

**Dosya içinde değişiklik varmı bakma-durumunu kontrol etme**<br/>
**Yeni bir dosya ekleyip git durumunda geçiş bölgesine eklenmediğini ve commit edilmediğini  gösterme**<br/>
`$ git status`

**Dosya içerisinde değişiklik olup olmadığını görme**<br/>
`$ git diff`

**Dosya içerisinden birşey silme**<br/>
`$ git rm main.py`

**Dosyayı ve içindekileri silme**<br/>
`$ git rm -r Silinecekler/`

**Dosya ismi değiştirme**<br/>
`$ git mv main.py deneme.txt`

**Dosya içine belge gönderme-taşıma**<br/>
`$ git mv deneme.txt Dosyalar/`

**Değişikleri geri alma**<br/>
**Yanlışlıkla silinen veya içinde değişiklikleri geri alma**<br/>
`$ git checkout -- index.txt`

**Versiyon Değiştirme**
**Geçilmek istenilen versiyonun şifleri kodu alınır sonuna (-- .) konulur**<br/>
`$ git checkout 3a51348a81552964ef4443219de52c9e0cc46899 -- .`

### GITHUB 
![github](https://image.flaticon.com/icons/svg/25/25231.svg)

**Githubdan oluşturulan repoya git ile dosya ekleme işlemi**<br/>
`$ git remote add githubRepo https://github.com/erncncbk/git-dersleri.git`

**Githuba gidip gitmediğini kontrol etme işlemi**<br/>
`$ git remote`

**Githuba gönderme işlemi(-u bütün dosyaları temsil eder)**<br/>
`$ git push -u githubRepo master`

***Git* ile Githuba yüklenilenleri silme işlemi**<br/>
`$ git rm main.py`

#### .gitignore  <br/>

**Githuba yüklerken dosyanın içerisinde yüklemesini istemediklerimizi .gitignore altında toplamalıyız**<br/>
*Örnek olarak veritabı klasörümün içerisindekileri yüklemek istemiyorum.<br/>
`$ cat >>.gittignore`
`veritabanı`

**.gitignore dosyasını açıp ekleme yapmak için**<br/>
`$ notepad .gitignore`

#### Branches (Dallar)

**Githubdan dal oluşturduktan sonra veya ekleme yaptıktan sonra veri çekmek için**<br/>
`$ git pull`

**Dal görüntüleme - oluşturma**<br/>
`$ git branch`
`$ git branch --all`

**Dal oluşturma ve master dalından oluşturulan dala gitme**<br/>
`$  git branch yandal2`
`$ git checkout yandal2`

**yandal2 de dosya oluşturma**<br/>
`$ touch yandal2.txt`

**master dalına geçme**<br/>
`$ git checkout master`


**master dalına geçme**<br/>
`$ git checkout master`

**master ve yandal2 arasındaki farkları görme**<br/>
`$ git diff master yandal2`

**master ile yandal2 yi birleştirme**<br/>
`$  git merge yandal2`

## Note
![note](https://image.freepik.com/freie-ikonen/ausrufezeichen-in-einem-kreis_318-9577.jpg)
<br/>
**Dosya içerisinde ekleme,silme veya değişiklik yapıldığında yapılması gerekenler!!**<br/>
*1-Durum kontrolü(herşey normalse sıkıntı yok)* <br/>
`$ git status` <br/>
*2-Değişiklik varsa geçiş bölgesine gönderme* <br/>
`$ git add .`<br/>
*3-geçiş bölgesindekileri commit etme*<br/>
`$ git commit -m "versiyonx"`<br/>
*4-Githuba gönderme*<br/>
`$ git push -u githubRepo master`



















