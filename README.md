# **Universiteti i Prishtinës**

# **Fakulteti i Shkencave Matematike-Natyrore**

# **Drejtimi Shkenca Kompjuterike**

![image1](https://user-images.githubusercontent.com/122290119/211401560-5ed55388-2cc7-47e6-a366-b5289a021c02.png)

## **Lënda: Programim për pajisje mobile**

#  Layout i aplikacionit

Layout i një aplikacioni i referohet rregullimit të elementeve vizuale
në një ekran ose faqe, të tilla si pozicioni dhe madhësia e elementeve
UI dhe struktura e një ndërfaqeje përdoruesi.

Ne kemi përdorur gjuhën skriptuese XML për layout-in e aplikacionit.
Aplikacioni ynë ka 5 layouts: activity_create_card.xml,
activity_main.xml, activity_splash_screen.xml, activity_update_card.xml,
view.xml.

Layout për aktivitetin CreateCard përdor një \`LinearLayout\` vertikal
për të rregulluar pamjet e saj fëmijë. \`LinearLayout\` ka një sfond të
zi dhe është vendosur të zërë gjerësinë dhe lartësinë e plotë të pamjes
së tij parent, me një mbushje prej 20 dp. Paraqitja ka një gravitet të
"qendrës" për të lidhur pamjet e fëmijës përgjatë boshteve vertikale dhe
horizontale.

Paraqitja përmban një 'TextView', dy pamje 'EditText' dhe një 'Button'.
"TextView" dhe dy pamjet "EditText" janë fëmijë të drejtpërdrejtë të
"LinearLayout". Pamjet \`EditText\` përdorin një sfond të personalizuar
\`@drawable/custom_edittetext\` për t'u dhënë atyre një pamje të
veçantë.

Këtu është një pamje:

![image2](https://user-images.githubusercontent.com/122290119/211401739-66a8fd31-fc8a-436f-91c1-0719c9ef5c83.png)



Figure 1: Paraqitja e CreateCard

Layout MainActivity përdor një \`LinearLayout\` vertikal si pamje
rrënjësore. \`LinearLayout\` ka një sfond të zi dhe zë gjerësinë dhe
lartësinë e plotë të ekranit.

Struktura përmban një "LinearLayout" të ndërthurur me një orientim
horizontal dhe një "FrameLayout". "LinearLayout" i ndërthurur përmban
një "TextView" dhe një "Button". "TextView" zë 1/2 e gjerësisë së
disponueshme dhe "Button" 1/2 tjetër. "FrameLayout" përmban një
"RecyclerView" dhe një "Button". "RecyclerView" merr gjerësinë dhe
lartësinë e plotë të "FrameLayout" dhe "Button" pozicionohet në qendër
të poshtme të "FrameLayout".

\`RecyclerView\` përdoret për të shfaqur një listë artikujsh dhe
plotësohet duke përdorur një skedar burimi të paraqitjes të quajtur
"view". "Butoni" "Shto" është një buton rrethor me një simbol "+" që
përdoret për të shtuar artikuj të rinj në listë. Butoni "deleteAll"
është një buton katror me një simbol "X" që përdoret për të fshirë të
gjithë artikujt nga lista.

Dhe kështu do të duket ky layout:
![image3](https://user-images.githubusercontent.com/122290119/211401822-301d9f2e-0198-4001-afa8-ef194e4e8914.png)



Figure 2: Paraqitja e MainActivity

Layout SplashScreen përdor një \`LinearLayout\` vertikal si pamje
rrënjësore. \`LinearLayout\` ka një sfond të zi dhe zë gjerësinë dhe
lartësinë e plotë të ekranit. Paraqitja është e përqendruar vertikalisht
dhe ka një gravitet "center_vertical".

Layout përmban dy elemente \`TextView\`. "TextView" i parë shfaq tekstin
"To Do" në të bardhë, me një madhësi fonti prej 40 sp dhe një familje
fonti sans-serif. "TextView" i dytë shfaq tekstin "Manage Your Day" në
një ngjyrë gri të çelur, me një madhësi fonti 16 sp, një hapësirë
shkronjash 0.3 dhe një familje fonti sans-serif. "TextView" i dytë është
rreshtuar horizontalisht duke përdorur gravitetin e paraqitjes
"center_horizontal" dhe ka një diferencë të lartë prej 10dp.

![image4](https://user-images.githubusercontent.com/122290119/211401892-cb84e923-a31a-43a4-a8fd-30999eba447d.png)

Figure 3: Paraqitja e SplashScreen

Layout UpdateCard përdor një \`LinearLayout\` vertikal si pamje
rrënjësore. \`LinearLayout\` ka një sfond të zi dhe zë gjerësinë dhe
lartësinë e plotë të ekranit. Paraqitja është e përqendruar vertikalisht
dhe ka një gravitet "qendër", me një mbushje prej 20 dp.

Paraqitja përmban një 'TextView', dy elemente 'EditText' dhe një
'LinearLayout' të ndërthurur me dy elemente 'Button'. \`TextView\` shfaq
tekstin "Update Details" në të bardhë, me një madhësi fonti 36 sp dhe
një familje fonti sans-serif. Elementet \`EditText\` përdoren për të
futur tekst dhe kanë një ngjyrë të bardhë teksti, me tekstin e aludimit
që ka një ngjyrë gri të çelur. "LinearLayout" i ndërthurur përmban dy
elementë "Button", me një orientim horizontal dhe një peshë prej 1 midis
tyre. Butoni i parë ka tekstin "Update" dhe butoni i dytë ka tekstin
"Delete" dhe një ngjyrë të kuqe sfondi.

![image5](https://user-images.githubusercontent.com/122290119/211401930-40d23bb1-ad3d-4b92-9ebf-d3b3283560d2.png)



Figure 4: Pamja e UpdateCard

Layout View përdor një \`LinearLayout\` vertikal si pamje rrënjësore.
\`LinearLayout\` ka një lartësi të përmbajtjes së mbështjelljes dhe zë
gjithë gjerësinë e ekranit. Ka një mbushje prej 7 dp.

Paraqitja përmban një element "CardView", i cili është një kartë e
dizajnit të materialit që ka një nuancë sfondi të zezë dhe një rreze
qoshe prej 10dp. "CardView" përmban një "LinearLayout" të ndërthurur me
një orientim vertikal. "LinearLayout" i ndërthurur përmban dy elemente
"TextView". "TextView" i parë ka një stil të theksuar, një madhësi fonti
24 sp, një ngjyrë të bardhë teksti dhe një familje fonti sans-serif.
"TextView" i dytë ka një madhësi fonti prej 15 sp, një ngjyrë të bardhë
teksti, një familje fonti sans-serif dhe një diferencë të lartë prej
5dp.

![image6](https://user-images.githubusercontent.com/122290119/211401988-348644bd-5ad5-408c-862b-7e76226b12d8.png)



Figure 5: Paraqitja e View

# Qëllimi i aplikacionit

Ky aplikacion do të ju ndihmojë përdoruesve të menaxhojnë detyrat e tyre
dhe të qendrojnë të

organizuar gjatë gjithë ditës. Features të aplikacionit “To-Do List App”

- Shtimi i një detyre të re në aplikacion

- Mundësia e shikimit të listës së detyrave

- Shënimi i një detyre si të përfunduar

- Vendosja e prioritetit

- Ndryshimi

- Fshirja

- Rifreskimi i listës së detyrave

- Klasifikim të detyrave në bazë të prioritet

# Arkitektura e aplikacionit 

Aplikacioni “TO DO LIST” përdor arkitekturën Model-View-ViewModel.

Diagrami 1: Arkitektura e aplikacionit

Në vazhdim do të shqyrtojmë klasat në Kotlin me anë të të cilave
aplikacionit i’a shtuam features e lartpërmendura.

Klasa \`CardInfo\` përdoret për të ruajtur informacionin në lidhje me
një detyrë në një listë detyrash. Ka dy veti: "title" dhe
"priority".Klasa \`CardInfo\` ka një konstruktor kryesor që merr dy
parametra: "title" dhe "priority". Këta parametra përdoren për të
inicializuar vetitë "title" dhe "priority" të objektit "CardInfo".

Klasa Adapter është një përshtatës i personalizuar RecyclerView që është
përgjegjës për shfaqjen e listës së detyrave në aplikacionin tonë të
listës së detyrave. Ai merr një listë të objekteve \`CardInfo\` si të
dhëna të tij dhe i përdor këto të dhëna për të mbushur elementet e
pamjes së secilit artikull në RecyclerView.

Klasa Adapter mbivendos metodat e mëposhtme:

\- \`onCreateViewHolder\`: Kjo metodë thirret kur RecyclerView duhet të
krijojë një mbajtës të ri pamjeje për të shfaqur një artikull. Ai fryn
paraqitjen për pamjen dhe kthen një mbajtës të ri pamjeje.

\- \`onBindViewHolder\`: Kjo metodë thirret nga RecyclerView për të
shfaqur të dhënat në pozicionin e specifikuar. Ai cakton ngjyrën e
sfondit të çdo artikulli bazuar në përparësinë e detyrës dhe cakton
tekstin për titullin dhe prioritetin TextViews. Ai gjithashtu vendos një
OnClickListener për çdo artikull që fillon aktivitetin UpdateCard kur
artikulli është klikuar.

\- \`getItemCount\`: Kjo metodë kthen numrin total të artikujve në
listën e të dhënave

Klasa CreateCard është një AppCompatActivity që lejon përdoruesin të
krijojë një detyrë të re me një titull dhe përparësi. Paraqitja për këtë
aktivitet përcaktohet nga layout activity_create_card. Butoni
save_button është vendosur të dëgjojë për klikime dhe kur klikohet,
kontrollon që create_title dhe create_priority të mos jenë bosh. Nëse
nuk janë bosh, ai ruan hyrjen në DataObject dhe fut një detyrë të re në
bazën e të dhënave duke përdorur objektin e bazës së të dhënave, i cili
është një shembull i klasës myDatabase. Në fund, fillon MainActivity.

Klasa DataObject është një objekt singleton që ruan një listë të
objekteve CardInfo. Ai siguron disa funksione për të manipuluar këtë
listë, duke përfshirë shtimin, fshirjen dhe përditësimin e elementeve në
listë, si dhe marrjen e të gjithë listës ose një elementi të vetëm nga
lista. Klasa CardInfo është një klasë e të dhënave që përbëhet nga dy
veti: titulli dhe prioriteti. Funksioni setData shton një objekt të ri
CardInfo në listë me titullin e specifikuar dhe vlerat e përparësisë.
Funksioni getAllData kthen të gjithë listën e objekteve CardInfo.
Funksioni deleteAll pastron listën e të gjithë elementëve. Funksioni
getData merr objektin CardInfo në pozicionin e specifikuar në listë.
Funksioni deleteData heq objektin CardInfo në pozicionin e specifikuar
në listë. Funksioni updateData përditëson titullin dhe vlerat prioritare
të objektit CardInfo në pozicionin e specifikuar në listë

Klasa Entity e cila përfaqëson një tabelë në bazën e të dhënave. Ka 3
fusha - id, titull dhe prioritet. Fusha id është çelësi kryesor i
tabelës dhe është vendosur të gjenerohet automatikisht. Titulli dhe
fushat prioritare janë vargje që përfaqësojnë titullin dhe përparësinë e
një detyre në tabelë. Shënimi @Entity specifikon që kjo klasë përfaqëson
një tabelë në bazën e të dhënave, dhe atributi i tabelës Emri specifikon
emrin e tabelës. Shënimi @PrimaryKey specifikon se fusha id është çelësi
kryesor i tabelës. Kjo klasë përdoret për të ruajtur dhe marrë të dhëna
nga baza e të dhënave.

Klasa MainActivity është një aktivitet Android që përdoret për të
shfaqur ekranin kryesor të aplikacionit. Ai inicializon bazën e të
dhënave duke përdorur Room dhe konfiguron dëgjuesit e klikimeve për
butonët add dhe deleteAll . Kur klikohet butoni add, aktiviteti nis
aktivitetin CreateCard. Kur klikohet butoni deleteAll, aktiviteti fshin
të dhënat e ruajtura në DataObject dhe gjithashtu fshin të gjitha të
dhënat e ruajtura në bazën e të dhënave duke përdorur funksionin
deleteAll të Objektit të Aksesit të të Dhënave të bazës së të dhënave
(DAO). Funksioni setRecycler thirret për të përditësuar RecyclerView me
të dhënat e reja. RecyclerView konfigurohet me një shembull të klasës
Adapter, së cilës i kalojnë të dhënat nga DataObject dhe një
LinearLayoutManager.

Klasa myDatabase është një klasë e bazës së të dhënave Room për një
aplikacion Android. Ai përfshin një metodë abstrakte dao() që kthen një
shembull të ndërfaqes DAO. Ndërfaqja DAO përcakton metodat për të hyrë
në bazën e të dhënave, të tilla si futja ose fshirja e të dhënave. Duke
përcaktuar këto metoda në ndërfaqen DAO, ne mund t'i përdorim ato në
pjesën tjetër të aplikacionit për të kryer operacionet e bazës së të
dhënave.

![image11](https://user-images.githubusercontent.com/122290119/211402041-b31594f1-cba5-4afa-96b8-ab3fd17a34cf.png)

Figure 6: Klasa myDataBase

Klasa SplashScreen është një AppCompatActivity që shfaq një splash
screen për 2 sekonda përpara se të nisë MainActivity. Ai gjithashtu
inicializon një bazë të dhënash Room dhe merr detyrat e ruajtura nga
baza e të dhënave për të mbushur fushën DataObject.listdata. Fusha
DataObject.listdata është një listë e ndryshueshme e objekteve CardInfo
që ruan detyrat që do të shfaqen në aplikacion.

![image12](https://user-images.githubusercontent.com/122290119/211402095-417d2e88-7511-498f-99d6-0224128ec590.png)

Figure 7: Paraqitja e klasës SplashScreen

Klasa UpdateCard është një aktivitet në aplikacion që lejon përdoruesin
të përditësojë ose fshijë një detyrë nga një listë. Shfaq një fushë
EditText për titullin e detyrës dhe një tjetër për prioritetin e
detyrës, si dhe një buton delete dhe një buton update. Kur klikohet
butoni delete, detyra hiqet nga lista dhe baza e të dhënave. Kur
klikohet butoni update, titulli dhe përparësia e detyrës përditësohen si
në listë ashtu edhe në bazën e të dhënave. Aktiviteti poashtu e kthen
përdoruesin në MainActivity kur klikohet një nga butonat.

Në aplikacionin “TO-DO List App” ne kemi përdorur DAO, e cila është
është një model dizajni që ofron një ndërfaqe abstrakte për një lloj
baze të dhënash ose mekanizma tjetër të qëndrueshmërisë.

Ndërfaqja DAO ofron metoda për aksesin dhe modifikimin e të dhënave në
bazën e të dhënave themelore.

myDatabase_Impl është një klasë që zgjeron klasën abstrakte myDatabase
dhe ofron një zbatim për të. Klasa myDatabase është një klasë e bazës së
të dhënave Room që shërben si një objekt aksesi në bazën e të dhënave
(DAO) për aplikacionin. Ai ofron metoda për leximin dhe shkrimin e të
dhënave nga baza e të dhënave dhe përcaktimin e skemës së bazës së të
dhënave. Klasa myDatabase_Impl përfshin një metodë createOpenHelper e
cila krijon dhe kthen një objekt SupportSQLiteOpenHelper që përdoret për
të menaxhuar bazën e të dhënave. Ai përfshin gjithashtu një metodë
createInvalidationTracker që krijon dhe kthen një objekt
InvalidationTracker që përdoret për të gjurmuar ndryshimet në të dhënat
në bazën e të dhënave. Së fundi, klasa myDatabase_Impl ka një metodë për
secilën nga metodat abstrakte të përcaktuara në klasën myDatabase. Këto
metoda ofrojnë zbatimin për operacionet e aksesit në bazën e të dhënave
të përcaktuara në klasën myDatabase.

Libraritë dhe frameworks e përdorura në aplikacion përfshijnë:

- Androidx Room: një librari për ofrimin e një shtrese abstraksioni mbi
  SQLite për të lejuar akses më të fuqishëm në bazën e të dhënave duke
  shfrytëzuar fuqinë e plotë të SQLite

- Kotlin Coroutines: një librari për menaxhimin e detyrave asinkrone në
  një mënyrë më të strukturuar, duke lejuar testimin dhe korrigjimin më
  të lehtë

- Androidx Lifecycle: një librari për të ndihmuar zhvilluesit të
  menaxhojnë ciklin jetësor të aktiviteteve dhe fragmenteve të tyre,
  duke përfshirë trajtimin e ndryshimeve të konfigurimit dhe ofrimin e
  një modeli pamjeje për të ruajtur të dhënat përgjatë ciklit jetësor të
  një aktiviteti ose fragmenti

- Androidx RecyclerView: një librari për shfaqjen efikase të grupeve të
  të dhënave të mëdha duke përdorur një listë lëvizëse dhe riciklimin e
  pamjeve ndërsa ato lëvizin jashtë ekranit

- Androidx ConstraintLayout: një librari për përcaktimin e paraqitjeve
  komplekse duke përdorur kufizime për të pozicionuar pamjet në lidhje
  me pamjet e tjera dhe paraqitjen mëmë

- Androidx AppCompat: një librari për ofrimin e përputhshmërisë për
  veçoritë më të reja në versionet më të reja të Android në pajisjet më
  të vjetra

# Rezultati

Kur klikojmë butonin "+", i cili na shfaqet në faqen e detyrave atëherë
n’a shfaqet pamja për të shtuar, përditësuar apo edhe fshirë ndonjë
detyrë e cila duket kështu:

![image13](https://user-images.githubusercontent.com/122290119/211402123-1f52241e-9340-40ad-8ef2-fc702bcbbb3f.png)


Figure 8: Kështu duhet të shtojmë një detyrë

Pasi shtojmë detyrat tona atëherë lista jonë e detyrave do të duket
kështu:

![image14](https://user-images.githubusercontent.com/122290119/211402156-22c2233a-83f2-4a95-bd64-ea964cede468.png)



Figure 9: Pamja e listës së detyrave

Nese klikojmë te një detyrë e caktuar atëherë do të mund t’a fshijmë atë
ose t’a përditësojmë, nëse e ndryshojmë tekstin e detyrës dhe e
ndryshojmë prioritetin dhe pastaj klikojmë butonin “Update” atëherë në
listën e detyrave do të n’a shfaqet lista e detyrave e përditësuar:

![image15](https://user-images.githubusercontent.com/122290119/211402196-109d33e2-9402-4886-ad98-05a3c73cada2.png)


Figure 10: Lista e detyrave e përditësuar

Nëse klikojmë butonin “Delete” atëherë ajo detyrë do të fshihet nga
lista jonë e detyrave:

![image16](https://user-images.githubusercontent.com/122290119/211402242-9bdc27f1-8596-4bc4-bb91-a8972c6a7427.png)




Figure 11: Lista e detyrave pasi e fshimë një detyrë

Nëse e klikojmë butonin “X” atëherë e gjithë lista e detyrave do të
fshihet:

![image17](https://user-images.githubusercontent.com/122290119/211402286-27c70114-5d6a-4edf-9ad9-5152543ae91f.png)



Figure 12: Pamja e listës së detyrave pasi klikojmë butonin “X”
