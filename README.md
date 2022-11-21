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

     🌑 Add a search engine where you could search for authors or specific recordings;

     🌒 The ability to create a playlist;
     
     🌓 The ability to change the profile picture;

*5. What differences do you see between testing a web application and a native one?* 


