# M++ Compiler

_Uwaga! Niniejsza **strona powstała w latach 2003-2005**. Niewiele jest jeszcze na czasie..._

M++ Compiler jest kompilatorem stworzonego przeze mnie języka M++. Podstawowym składnikiem pakietu jest wsadowy kompilator "mpp.exe". Nie posiada on własnego edytora, przez co kod programu należy przygotować w dowolnym innym programie zapisujacym pliki w formacie TXT (chociażby Notatnik z Windows).

Pliki skompilowane za pomoca M++ Compiler mają format COM, przez co moga być uruchamiane w dowolnym środowisku kompatybilnym z systemem DOS. Należy pamiętać, że pliki typu COM nie mogą być większe niż 64 kB!

W skład pakietu wchodzi także konwerter plików "com2exe.exe", który zamienia pliki COM na pliki EXE.

Język posiada bardzo prostą składnie wzorowana na językach Pascal, C++ oraz Assembler. Wszystkie jego instrukcje są tak zaprojektowane, że prędkością dorównuja 32-bitowemu Assemblerowi.

Pełna wersja pliku pomocy wraz z opisem wszystkich elementów języka M++ dostępna jest [tutaj](download/compilers/mpp_v1-5a.pdf).

Jedna z wersji M++ Compiler otrzymała wyróżnienie w finale XII edycji Kaliskiego Konkursu Informatycznego, inna zakwalifikowała się do finału XIII edycji.

[Pobierz](https://michzimny.pl/download/compilers/mpp_v1-5a.rar)

### Historia wersji

**1.5a** (23.01.2005)  
\- wprowadzono zmienne (byte i char)  
\- zmieniono sposób zapisu programu do pliku COM  
\- zmieniono nazwy niektórych instrukcji (np. pętli)  
\- usunięto instrukcje Readkey, Write i GotoXY (pozostały ich odpowiedniki: get, put i nl)  
\- wprowadzono skok do etykiety  
\- poprawiono procedurę wait  
\- wprowadzono obsługę zmiennych przez instrukcje put i get

**1.4** (02.10.2004)  
\- wprowadzono dyrektywy kompilatora  
\- dodano dyrektywę !E  
\- dodano instrukcje put i nl

**1.3** (24.09.2004)  
\- dodano pętle  
\- dodano instrukcje stc (SeT Counter)  
\- ulepszono instrukcję REP  
\- dodano instrukcje GotoXY

**1.2+** (25.08.2004)  
\- ulepszono instrukcje REP o obsługę większej ilośći instrukcji  
\- można używać etykiety "Label" przy skoku pętli REP

**1.2** (23.08.2004)  
\- dodano pętle nieskończoną - instrukcje REP

**1.1** (30.06.2004)  
\- umożliwiono wprowadzanie do instrukcji więcej niż jednego parametru (maks. 5)  
\- dodano możliwość wyświetlania pikseli  
\- dodano instrukcje skoku bezwarunkowego

**1.0b** (21.05.2004)  
\- dodano możliwość używania tzw. "białych znaków" w dowolnych miejscach kodu  
\- poprawiono odczytywanie parametrów tekstowych  
\- zmieniono algorytm wyświetlania tekstu  
\- wprowadzono uruchamianie trybów SVGA  
\- wprowadzono obsługę głośnika systemowego  
\- poprawiono użycie instrukcji kodu maszynowego (HEX=MCI)  
\- zmieniono procedury 16-bitowe na 32-bitowe

**1.0a** (27.03.2004)  
\- poprawienie obsługi programu  
\- usunięcie niedoróbek

**0.8b** (6.01.2004)  
\- dodanie wyświetlania tekstu (ciągów znaków)

**0.7** (4.01.2004)  
\- dodano wybieranie pliku metodą Drag&Drop  
\- poprawiono obsługę plików przez kompilator

**0.6+** (22.12.2003)  
\- poprawiono obsługę ekranu w trybie tekstowym

**0.6** (22.12.2003)  
\- dodano konwerter plików COM na EXE  
\- dodano obługę ekranu w trybie tekstowym

**0.5b** (20.12.2003)  
\- poprawiono obsługę wszystkich trybów VGA

**0.4a** (19.12.2003)  
\- dodano obsługę wszystkich trybów VGA  
\- poprawiono obsługę błędów

**0.3+** (15.12.2003)  
\- dodano obsługę trybów VGA (03h i 13h)

**0.3a** (15.12.2003)  
\- dodano obsługę ekranu w trybie graficznym  
\- dodano obsługę kodu maszynowego (HEX)

**0.1 ... 0.2** (xx.12.2003)  
\- powstawanie kompilatora  
\- obsługa klawiatury