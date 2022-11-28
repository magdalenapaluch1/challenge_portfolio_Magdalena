# **Challenge_Portfolio_Magdalena**

# **Task 1**
## Subtask 1
Podczas testu wiedzy zdobyłam 9 punktów. 🏆
## Subtask 3
Cześć świecie DareIT! :upside_down_face:

Nazywam się Magda i od dłuższego czasu staram się wejść w świat testowania. Droga jest dość wyboista, jednak bardzo interesująca. 
Wziełam udział w projekcie, bo lubię nowe wyzwania. Od naszych cotygodniowych spotkań i zadań oczekuję ogromu praktycznej wiedzy, 
która pozwoli mi poczuć się jak w prawdziwym projekcie. Jestem zaciekawiona i z niecierpliwością będę wyczekiwać kolejnych tasków. :)
## Subtask 4

**Aplikacja którą testujemy: https://scouts-test.futbolkolektyw.pl/pl**

*1. Do czego służy aplikacja?*

   Aplikacja służy do gromadzenia informacji o graczach/piłkarzach. 
   Znajdziemy w niej szczegółowe informacje o konkretnym piłkarzu (pochodzenie, pozycja, cechy fizyczne itp.). 
   Każdy gracz ma przypisaną historię meczy, w których grał oraz użytkownik ma możliwość sprawdzenia sumarycznych raportów z meczów.
   Raporty można uzupełniać o szczegółowe informacje dotyczące zachowania zawodnika na boisku.
    
*2. Jakie funkcjonalności ma aplikacja?*

   **W aplikacji można wyróżnić następujące funkcjonalności:**
   * Dodawanie gracza do listy; 
   
     *UWAGA: Opcja dodania gracza z widoku zakładki gracze, byłaby wygodna i intuicyjna.*
     
     *UWAGA: Możliwość edycji informacji o zawodniku nie powinna być dostępna po naciśnięciu w konkretny wiersz (imię i nazwisko gracza), 
             uważam że powinna się wyświetlać strona, która jest podsumowaniem, a nie edycją. Opcja edycji mogłaby być dostępna tylko dla autora rekordu.*
   * Dodawanie i edycja informacji o meczu, które są przypisane do określonego gracza;
   
     *UWAGA: Możliwość wejścia do zakładki "Mecze" z menu głównego, byłaby wygodna i intuicyjna.
             Ktoś może znać informacje z meczu i chcieć kogoś znaleźć, bez znajmości imienia i nazwiska gracza.*
   * Ściąganie listy graczy w postaci plików .CSV, poprzez naciśnięcie odpowiedniej ikony;
   * Wydruk listy graczy, poprzez naciśnięcie odpowiedniej ikony;
   * Możliwość zmiany wyświetlanej tabeli z graczami (np. ukrywanie kolumn), poprzez naciśnięcie odpowiedniej ikony;
   * Filtrowanie listy graczy, poprzez naciśnięcie odpowiedniej ikony;
   
      *UWAGA: Powinna być dostępność podstawowych filtrów, czyli sortowanie alfabatyczne, rosnące, malejące (np. wiekiem, ilością meczy, raportów).*
   * Możliwość wyszukiwania zawodników.
    
*3. Interfejs aplikacji*

   * Strona jest prosta, nie za bardzo rozbudowana. Na pierwszy rzut oka, na stronie głównej nawigacja wydaje się łatwa i przejrzysta.
   * Kafelki u góry strony informują nas o liczbie graczy, meczy, raportów, akcji, jednak nie są one interaktywne i nie nawigują do konkretnych zbiorów. 
   * Nie ma możliwości prześledzenia meczy, ponieważ dostępna jest tylko zakładka Graczy.
   * Przechodząc dalej w menu boczne, w zakładkę "Gracze", brakuje spójności. Nie jest jasne czy istnieje możliwość kliknięcia w konkretnego gracza, 
     zobaczenia jego danych, czy edycji informacji.
   * Zaletą aplikacji jest dostępność tłumaczenia na jezyk angielski.
   * Tekstury i kolory są poprawne, nie są jaskrawe, nie atakują użytkownika i nie rozpraszają jego uwagi.
   * Pojawiają się powiadomienia, które informują użytkownika o zmianach na stronie (np. dodając nowego zawodnika).
   * Strona jest dostępna na urządzeniach moblinych.
   * Korzystając z DevTools Lighthouse przeglądarki Chrome, Performance dla urządzeń mobilnych jest niższy (ok. 75), niż dla przeglądarek desktopowych (ok. 88).

*4. Intuicyjność*

   Z poziomu strony głównej wszystko jest jasne. Występuje opcja "Dodaj gracza", widać które informacje odsyłają nas do kolejnych podstron.
   Z poziomu zakładki "Gracze" brak możliwości dodania nowego gracza. Mogłaby pojawić się opcja dodania gracza w tym oknie, 
   przycisk z plusem, jako dodanie nowego gracza. Taka opcja występuje w podstronie z meczami i raportami.
   Na stronie głownej pojawiają się informacje o ilości graczy, meczy, raportów, jednak opróczzawodników nie możemy niczego innego przeglądać.
   Powinna pojawić się opcja wejścia we wszystkie mecze i raporty, np. z bocznego menu, tam gdzie znajduje się opcja "Gracze".
   Brak możliwości usuwania graczy/meczy z listy. 

*5. Błędy*

   * "Niepoprawne ściąganie listy graczy w postaci pliku .CSV"
   
      Rezultat: Ściągnięcie listy graczy tylko z aktualnie otwartej strony spisu zawodników (10 rekordów).
   
      Oczekiwany rezultat: Ściągnięcie całej bazy zawodników.
   
      Priorytet: niski
   
      *Komentarz: Mam na uwadzę sytuację, że taka funkcjonalność mogła zostać tak zaprojektowana, 
                  jednak ze względu na użyteczność wydaje mi się, że wygenerowanie raportu z listą dostępnych graczy w całości,
                  byłoby bardziej optymalne (przeniesienie do innej aplikacji/bazy).*
                  
   * "W sekcji "Gracze" po najechaniu na zawodnika nie wyświetla się odsyłacz do indywidyulanej strony"
   
      Rezultat: Najechanie na wiersz z graczem nie wskazuje na możliwość kliknięcia.
   
      Oczekiwany rezultat: Pojawienie się odsyłacza do indywidualnej strony zawodnika.
   
      Priorytet: niski
   
   * "Po dodaniu gracza przekierowuje nas na stronę edycji"
   
      Rezultat: Po uzupełnieniu informacji o graczu, którego dodajemy do systemu, pojawia się informacja o dodaniu i przekierowaniu do opcji edycji.
   
      Oczekiwany rezultat: Przekierowanie na stronę z ogólnym profilem gracza.
   
      Priorytet: średni
      
   * "Podczas edycji raportu z meczu, wprowadzaniu zmian, przycisk "SAVE" nachodzi na sekcję "Dodatkowy komentarz"
   
      Rezultat: Po uzupełnieniu informacj o meczu, przycisk "SAVE" nachodzi na inne pola tekstowe.
   
      Oczekiwany rezultat: Przycisk "SAVE" pozostaje w jednym miejscu.
   
      Priorytet: średni
      
   * "W oknie "Rozpocznij mecz" można rozpocząć więcej niż 2 połowy meczu."
      
      Rezultat: Po uruchomieniu meczu, klikając z przycisk zegarka, można ustawić większą liczbę połów niż dwie.
   
      Oczekiwany rezultat: Dostępne są tylko dwie połowy meczu.
   
      Priorytet: wysoki
      
  * "W oknie dodawania gracza, przycisk "Clear" nie usuwa informacji z formularza."
      
      Rezultat: Po kliknięciu w przycisk "Clear" w formularzu edycji informacji o graczu, nie następuje usunięcie danych.
   
      Oczekiwany rezultat: Usunięcie danych w formularzu.
   
      Priorytet: średni
      
   * "Możliwość dodania gracza bez danych"
      
      Rezultat: Stworzenie konta gracza, po wpisaniu SPACJI w puste pola.
   
      Oczekiwany rezultat: Informacja o konieczności wypełnienia pustego pola ciągiem znaków, cyfr.
   
      Priorytet: wysoki 
      
   **Ogólny komentarz:**
   
   Sekcja dodawania graczy i wszystkie pola do uzupełnienia powinny być zablokowane przed wpiasaniem niepoprawnych danych.
   
   Puste pola lub pola ze spacją, abstrakcyjne wartości wagi i wzorstu, daty, powinny być blokowane przed wpisaniem niepoprawnej danej
   np. litery w pola numeryczne (numer telefonu).
   
   Brakuje profilu osoby zalogowanej, gdzie moglibyśmy sprawdzić ile osób dodaliśmy do bazy, gdzie widniałyby nasze dane.
   
   W oknie logowania, w polu "Login" powinna się pojawić informacja, że konieczne jest wpisanie adresu e-mail.
   
# **Task 2**
## Subtask 1

🍀 [Test Case's based on User Stories](https://docs.google.com/spreadsheets/d/1Mt6FQfttUFqRPDLyb7hc2ceToqsZNYIl9pZsS1tunlI/edit?usp=share_link) 

## Subtask 2

💡 [Mind map](https://drive.google.com/file/d/1Ss96V3r3SxSOSsJsx9XGYkWmtub9qNM9/view?usp=sharing) 

🍀 [Test Case's based on experience_Website in English 🇺🇸](https://docs.google.com/spreadsheets/d/1589dqUD6PTWXDCuFfejT0MtGR948kEbCJlDr_RXLel8/edit?usp=sharing) 

🍀 [Test Case's based on experience_Website in Polish 🇵🇱](https://docs.google.com/spreadsheets/d/1_b5FHHD66fsbNYWxK1uss5EWN4cLvsm8mHx3zcd7j2g/edit?usp=sharing)

## Subtask 3
[Po co piszemy Test Case'y, komu to potrzebne? / Why are we writing Test Cases, who needs them?](https://www.youtube.com/watch?v=OO3FANjwKHY&t=1s) 🙈

Test cases are important to systematize what we plan to do / test.

Test cases allow us to determine the functionality coverage.

We can create them at the stage when the product documentation is not yet fully ready, 
by the principle that **Early testing saves time and money**.

Test cases help get to know the application.

Test cases find defects in the product.

# **Task 3**
## Subtask 2

💡 [Mind map](https://drive.google.com/file/d/1Ss96V3r3SxSOSsJsx9XGYkWmtub9qNM9/view?usp=sharing) 

🍀 [Test Case's based on experience_Website in English 🇺🇸](https://docs.google.com/spreadsheets/d/1589dqUD6PTWXDCuFfejT0MtGR948kEbCJlDr_RXLel8/edit?usp=sharing) 

🍀 [Test Case's based on experience_Website in Polish 🇵🇱](https://docs.google.com/spreadsheets/d/1_b5FHHD66fsbNYWxK1uss5EWN4cLvsm8mHx3zcd7j2g/edit?usp=sharing)

## Subtask 3

📈📉 [Test Report](https://drive.google.com/file/d/1VGMOqnqYJ60v0evxkWfCRPHHpuTganN6/view?usp=sharing)

# **Task 4**
## Subtask 2

🪳 [Bug Report](https://docs.google.com/spreadsheets/d/1HwSalkbEryYPYpr7G_5F2mwVYxa2ND41hCxHNOjhizE/edit?usp=sharing)

## Subtask 3

*1. What is this app for? What is the purpose of this app?*

💡 The Focusly app focuses on learning how to meditate and breathe properly. 

   Podcasts and recordings allow you to calm down, improve creativity, fight with lack of concentration, anxiety or bad sleep.
    
   It helps to achieve the goals selected in the application and builds the habit of regularity.

*2. Who is going to be the end user of the application?*  

💆‍♀️💆The end user of this application can be any person who wants to learn to meditate or people who already have some experience in meditating.

*3. Do you think the application is user friendly?* 

🍀 The application has a friendly look, the colors are subdued, they don't attack the user. 

   The application doesn't consume too much energy, it can be run in the background. 
   
   The application doesn't have its equivalent in the form of a website where data could be synchronized. 
   
   The advantage of the application is the ability to delete an account from the application level.

*4. How would you improve the application? What would you improve about it? Do you have any idea for additional functionality?*

🌚As an additional functionality I would introduce:

   🌕 The ability to set the playback speed;

   🌖 The ability to scroll through the lessons with your finger (swipe right - swpie left for next lessons or previous);

   🌗 In breathing tasks, add the possibility of obtaining a sound that tells us to inhale, exhale;

   🌘 The first time when user enter the application, add a tutorial (understand what to do with the app);

   🌒 The ability to create a playlist;
     
   🌓 The ability to change the profile picture;
     
   🌔 Availability of foreign-language podcasts in the Polish version of the application without changing the language

*5. What differences do you see between testing a web application and a native one?* 

When we are testing web applications, we can receive information from the server in the form of code. 
Testing web applications takes place in different browsers, while testing mobile applications takes place on different devices with different operating systems. 
In testing mobile applications, we can take into account factors such as: battery levels, push notifications, sensors built into the device.

# **Task 5**
## Subtask 1

📊✒️Finished course "Kurs SQL od podstaw"](https://www.udemy.com/course/kurs-sql-od-podstaw/)

**Typ zapytania:**
SELECT/INSERT/UPDATE/DELETE - typ zapytania

1. **FROM** - źródło pobrania danych
2. **WHERE** - warunek
3. **GROUP BY** - grupowanie rekordów
4. **ORDER BY** - sortowanie

**SELECT** - wybieranie danych z bazy danych

*SELECT column1, column2, ... FROM table_name;*

**SELECT DISTINCT** - zwraca tylko odrębne wartości, zwraca unikalne wartości, bez duplikatów

*SELECT DISTINCT column1, column2, ... FROM table_name;*

**WHERE** - filtruje rekordy, po zadeklarowaniu warunku

*SELECT column1, column2, ... FROM table_name;*
*WHERE condition;*

**Operatory AND, OR, NOT**

**AND** - wszystkie warunki muszą być prawdą

**OR** - którykolwiek warunek jest PRAWDZIWY

**NOT** - nieprawdziwy warunek

**IS NULL** - równa zero, pusta kolumna

**IS NOT NULL** - nie jest równa zerem, pełne kolumny

**TOP** - liczba rekordów do zwórcenia

**LIMIT** - obsługiwany przez MySQL

*SELECT column1, column2, ... FROM table_name*
*WHERE condition1 AND condition2;*

*SELECT column1, column2, ... FROM table_name*
*WHERE condition IS NULL;*

*SELECT TOP number column_name(s) FROM table_name*
*WHERE condition1;*

*SELECT column_name(s)FROM table_nameWHERE condition LIMIT number;*

**MIN()** najmniejsza wartość z wybranej kolumny

**MAX()** największa wartość z wybranej kolumny

*SELECT MIN (column_name) FROM table_name WHERE condition1;*

**COUNT()** - podaje liczbę wierszy spełniających warunek

*SELECT COUNT (column_name) FROM table_name WHERE condition1;*

**AVG()** - zwraca średnią wartość kolumny numerycznej

*SELECT AVG (column_name) FROM table_name WHERE condition1;*

**SUM()** - całkowita suma kolumny numerycznej

*SELECT SUM (column_name) FROM table_name WHERE condition1;*

**LIKE** - w klauzuli WHERE, do wyszukiwania określonego wzorca

*SELECT column1, column2, ... FROM table_name WHERE columnN LIKE pattern;*

**BETWEEN** - wybiera wartości z danego zakresu.

*SELECT column_name(S) FROM table_name WHERE column_name BETWEEN value1 AND value2;*

**Aliasy** - nadawanie kolumnie w tabeli tymczasowej nazwy, 
nazwa ta zostaje na czas aktualnego zapytania

*SELECT column_name AS alias-name FROM table_name;*

**ORDER BY** - sortowanie zestawu wyników w kolejności rosnącej lub majlejące
rosnąco **ASC**, malejąco **DESC**

*SELECT column1, column2, ... FROM table_name ORDER BY column1, column2, ... ASC|DESC;*

**Pokazanie całej zawartości tabeli:**

*SELECT * FROM categories;*

* - to ALL

Wyszukiwanie stringów zawsze w cudzysłowie

**%** oznacza dowolną literę
**_** pozwoli wskazać konkretne miejsce litery w wyrazie

**INSERT INTO** - służy do wstawiania nowych rekordów do tabeli

*INSERT INTO Customers (CustomerName, City, Country) VALUES ('Cardinal', 'Stvanger', 'Norway');*

**UPDATE** służy do aktualizacji istniejących rekordów  w tabeli

*UPDATE Customers SET ContactName = 'Alfred Schmidt', City = 'Frankfurt' WHERE CustomerID = 1*

**DELETE** - służy do usuwania istniejących rekordów w tabeli

*DELETE FROM Customers WHERE CudtomerName = 'Alfreds Futterkiste'*

**GRUOP BY** pozwala na grupowanie rekordów według róznych zasad

*SELECT COUNT (CustomerID), Country FROM Customers GROUP BY Country;*

**HAVING** zwraca podsumowanie dla całej tabeli, wywołana funkcja GROUP BY

*SELECT COUNT (CustomerID), Country FROM Customers GROUP BY Country; HAVING COUNT (CustomerID) >5;*

**INNER JOIN** łączenie wierszy z conajmniej dwóch tabel na podstawie powiązanej między nimi kolumny

*SELECT Orders.OrderID, Customers.CustomerName FROM Orders INNER JOIN Customers ON Orders.CustomerID=Customers.CustomerID*

**LEFT JOIN** zwraca wszystkie rekordy z lewej tabeli oraz pasujące rekordy z prawej tabeli

*SELECT column_name(s) FROM table1 (lewa tabelka) LEFT JOIN table2 (prawa tabelka) ON table1.column_name = table2.column_name*

**RIGHT JOIN** zwraca wszystkie rekordy z prawej tabeli oraz pasujące rekordy z lewej tabeli

*SELECT column_name(s) FROM table1 (prawa tabelka) RIGHT JOIN table2 lewa tabelka) ON table1.column_name = table2.column_name*

**UNION** służy do łączenia zestawu wyników dwóch lub więcej instrukcji SELECT

*SELECT column_name(s) FROM table1 UNION SELECT colu(s) FROM table2*

