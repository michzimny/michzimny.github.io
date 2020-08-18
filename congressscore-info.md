# CongressScore

Aktualna wersja stabilna: **1.3.4** oraz **1.3.6** (02.05.2010)

Zainteresowany? [Pisz!](/contact)

Program służy do obliczania wyników klasyfikacji długofalowych. Dwa sposoby liczenia: suma PDF lub suma procentów. Dane turniejów pobierane są z plików \*.csv w formacie [MSC CEZAR](http://www.msc.com.pl/cezar), generowanych przez programy liczące (m.in. [KoPS](http://kops.com.pl/) czy [Teamy](http://www.pzbs.pl/pary-teamy) J.Romańskiego (\*)).

**Program policzy także szybko klasyfikacje klubów, miast, szkół itp!!**

*   [plik pomocy](download/CongressScore.pdf)
*   [Congress Score na Windowsie 64-bitowym](/congressscore-x64)

Główne możliwości programu:

*   wyniki generowane do formatu html, umożliwiającego łatwe opublikowanie ich w Internecie lub wydruk na drukarce
*   długa fala z pełnymi informacjami (imię, nazwisko, wk, okręg, informacja junior/senior itp, możliwy także klub); przy tym brak problemów z rozróżnianiem zawodników o tych samych nazwiskach i inicjałach imion, jak w powszechnie używanym dotychczas programie do długiej fali
*   modyfikowana liczba zaliczanych zawodnikowi wyników
*   możliwość zdefiniowania priorytetów dla poszczególnych turniejów, rozstrzygających w przypadku zajęcia miejsc ex-aequo
*   zaliczanie turniejów ze względu na typ (np. zaliczane: 3 z 5 na maksy, 2 z 3 na impy, teamy, indywiduel)
*   liczenie klasyfikacji grupowych: klubów, miast, szkół itp.

Wynik działania programu:

*   [49\. Poznański Kongres Brydżowy](http://kongres.brydz.wlkp.pl/wyniki2009/congressscore.html)
*   [Grand Prix Wielkopolski 2009](https://michzimny.pl/bridge/2009/gpw/congressscore.html)
*   [Grand Prix Dąbrówki 2008/09](https://michzimny.pl/bridge/2009/gpdabrowki/congressscore.html)
*   [52\. Międzynarodowy Kongres Brydżowy w Sławie](http://stara.pzbs.pl/wyniki/2009/krajowe/gpp/09slawa/wyniki/pdfex.html)
*   [KLASYFIKACJA KLUBÓW na MPJ 19-20](http://stara.pzbs.pl/wyniki/2009/mlodziez/mpj09/kkk.html)

Wymagania:

*   [Microsoft .NET Framework 2.0](https://www.microsoft.com/downloads/details.aspx?FamilyID=0856eacb-
    4362-4b0d-8edd-aab15c5e04f5)
*   [Serwer MySQL (w wersji co najmniej 5.0; zalecana 5.1)](https://www.mysql.com/)
*   **separator dzięsiętny: . (kropka) - należy zmienić w Ustawieniach regionalnych**
*   zobacz **[Congress Score na Windowsie 64-bitowym](/congressscore-x64)**

\* - Jeszcze drobna uwaga do najpopularniejszych programów liczących. Plik .csv wczytywany do Congress Score'a musi być zgodny ze specyfikacją, tzn. dziewiąta jego kolumna zawiera klub (dla CS'a raczej nieistotne), a dopiero dziesiąta zawiera PDFy.  
KoPS generuje csv w ten sposób wtedy, gdy w kops.ini opcja  
\[CSVKLUBPDF\] \* zapisuj klub i pdf do csv, TAK lub NIE  
jest ustawiona na TAK; natomiast Teamy generują csv z pdf-ami poprawnie dopiero od wersji 5.0.29. W przypadku korzystania z wersji poprzednich należy odpalić \*.csv w Excelu i dodać ew. brakujące kolumny (mogą być puste), tak by PDFy znalazły się w kolumnie dziesiątej (kolumna J).

Zainteresowany? [Pisz!](/contact)

### Historia wersji

**1.3.4** (02.05.2010)

*   pdfy mogą być niecałkowite (suma zaokrąglana do dwóch miejsc po przecinku)

**1.3.3** (31.03.2010)

*   poprawiona obsługa csv (problem średnika wewnątrz pola)
*   poprawiony bug przy liczonych=0 w klasyfikacjach klubowych (występował tylko w 1.3.2)
*   poprawki kosmetyczne

**1.3.2** (22.11.2009)

*   w klasyfikacjach grupowych możliwość zmiany liczby zaliczanych najlepszych zawodników z danej grupy
*   poprawki kosmetyczne

**1.3.1** (13.10.2009)

*   dodano przycisk "usuń bazę/falę" w okienku "Otwórz"
*   poprawiono bug z użyciem pojedyńczego apostrofu w Logoh'u
*   poprawiono bug z wyjściem z okienka "Nowa" bez tworzenia nowej fali
*   poprawki kosmetyczne

**1.3** (01.10.2009 _oraz wcześniejsze RC_)

*   STARE KLASYFIKACJE NIE DZIAŁAJĄ - aby działały, trzeba na nich wykonać [te zapytania](download/1.2.6-1.3.0.txt)
*   możliwość definiowania grup turniejów - np. liczone 3 najlepsze na maksy, 2 najlepsze na impy, zawsze indywiduel i zawsze KMP
*   liczenie klasyfikacji klubów, miast, szkół etc.
*   działa alt+tab jak jest otwarte "pod-okienko"
*   poprawiona obsługa wyjątków przy wczytywaniu turnieju

**1.2.8** (30.08.2009)

*   funkcja "podmień turniej"
*   poprawiony bug z naciśnięciem enter w okienku "logoh"
*   poprawiony błąd przy N(X) i nieistniejącym w bazie zawodniku (tzn. są punkty, nie ma nazwiska)

**1.2.6** (14.08.2009)

*   wagi zostały przemianowane na priorytety  
    teraz może istnieć dowolna liczba turniejów o priorytecie 0 oraz maksymalnie jeden turniej o priorytecie N, dla każdego N>0
*   dodano port do ustawień MySQL
*   poprawiony drobny bug z blokowaniem się pola "liczonych turniejów" jeśli próbowaliśmy tam coś wpisać, a żaden turniej nie był jeszcze wczytany
*   zawodnicy, którzy zajęli miejsca ex-aequo, są posortowani alfabetycznie (dotychczas zdarzały się wyjątki od tej reguły)
*   poprawiony plik pomocy

**1.2.5** (28.07.2009)

*   poprawka drobnego bug'a niepozwalającego dodać zawodnika w niektórych sytuacjach po wcześniejszej ręcznej edycji bazy lub usunięciu niektórych turniejów
*   dodatkowe zabezpieczenie w funkcji transferu punktów między zawodnikami
*   rozszerzenie pola shortname (wszystkie stare klasyfikacje działają prawidłowo)

**1.2.4** (26.07.2009)

*   dodano trochę zabezpieczeń przed błędami wynikającymi z niewłaściwej, ręcznej edycji bazy
*   dodana możliwość transferu punktów między zawodnikami
*   możliwość ustawienia by program brał pod uwagę, że wczytywani z \*.csv niezrzeszeni mogą mieć imiona i nazwiska pozbawione polskich znaków (taka sytuacja się nie zdarzy jeśli zawsze używamy KoPS+WinLista, Teamy itp.) - jeśli chcesz skorzystać z tej funkcji KONIECZNIE zapoznaj się z jej [instrukcją](download/cs_bez_polskich.txt)

**1.2.2** (25.07.2009)

*   od razu po wczytaniu turnieju pojawia się okienko umożliwiające wprowadzenie nazwy, wagi czy linku turnieju
*   z okienka dodawania niezrzeszonych znika opcja "pomiń"
*   jeżeli zawodnik jest niezrzeszony i nie ma w bazie żadnego o tym samym imieniu i nazwisku, to przy wczytywaniu turnieju program o takiego nie pyta - taki zawodnik jest od razu dodawany do bazy jako nowy; pytanie pojawia się tylko, jeśli w bazie są już jacyś zawodnicy o tym samym imieniu i nazwisku; (po wczytaniu turnieju pojawia się lista zawodników dodanych do bazy automatycznie)
*   liczba zaliczanych turniejów może być zdefiniowana z góry na np. 10, mimo że wczytanych turniejów jest tylko 5 (wcześniej było to niemożliwe)

**1.2.1** (21.07.2009)

*   poprawione problemy z kodowaniem przy domyślnym kodowaniu bazy innym niż latin2
*   drobiazgi techniczno-kosmetyczne

**1.2** (19.07.2009)

*   poprawiony błąd z kodowaniem
*   wczytywanie bazy zawodników na 3 sposoby: bezpośrednio z Internetu (Cezar), lokalnie z pliku baza.csv, z JFR Teamy; możliwość aktualizacji bazy
*   poprawiona obsługa wyjątków MySQL
*   logoh edytowane bezpośrednio w programie
*   nagłówki kolumn z nazwami poszczególnych turniejów w html mogą być linkami do wyników
*   aby klasyfikacje stworzone w poprzednich wersjach działały z bieżącą to na każdej należy wykonać:  
    ALTER TABLE \`tournaments\` ADD COLUMN \`link\` varchar(100) default NULL;

**1.1.2** (15.07.2009)

*   gdy wystąpi błąd przy wczytywaniu turnieju to w \`data\` zostają "osierocone" rekordy - pojawił się przycisk do ich łatwego usuwania ("usuwanie błędów")
*   poprawione drobiazgi z wyświetlaniem float-ów (w wariancie z sumowaniem procentów)

**1.1** (13.07.2009)

*   lekko poprawiona obsługa błędów
*   drobny bug z wk (bo czasem "0", czasem "0.0" a czasem "null")
*   poprawiony problem z podawaiem wszystkich danych (klucz i dane MySQL) przy każdej zmianie programu (nowa wersja, przeniesienie pliku)
*   instalka

**1.0.4** (10.07.2009)

*   logoh czytane z bazy tylko gdy potrzebne (nie trzymane w programie)
*   dynamiczny colspan w empty.html (zazwyczaj trochę za duży, ale przeglądarki sobie radzą)
*   opcjonalna kolumna "pierwszy do poprawki" - N(X), gdzie N - liczba turniejów, w których zawodnik zapunktował, X - pierwszy wynik do poprawki
*   opcje turniejów (shortname, waga, pokazywanie na wydruku) edytowalne z poziomu programu

**1.0.2** (05.07.2009)

*   drobiazgi kosmetyczne dla ŁK
*   kolumna \`show\` w \`tournaments\` (czy pokazywać dany turniej na wydruku)

**1.0.1** (04.07.2009)

*   zmiany kosmetyczne
*   wydruk wyników albo z logoh z \`admin\` albo z \[h2\]NAZWA DLUGIEJ FALI\[/h2\] (jak generujemy wyniki do wywieszenia na ścianie to często nie chcemy w nagłówku mieć całego logoh'a)

**1.0** (03.07.2009)

*   pierwsza, w pełni działająca wersja

**0.1 - 0.4.5** (do 14.06.2009)

*   powstawanie programu, ale da się używać go już do liczenia (vide: kongres poznański)
