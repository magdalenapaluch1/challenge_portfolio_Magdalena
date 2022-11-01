# **Challenge_Portfolio_Magdalena**

# **Task 1**
## Subtask 1
Podczas testu wiedzy zdobyłam 9 punktów.
## Subtask 3
Cześć świecie DareIT! :upside_down_face:

Nazywam się Magda i od dłuższego czasu staram się wejść w świat testowania. Droga jest dość wyboista, jednak bardzo interesująca. 
Wziełam udział w projekcie, bo lubię nowe wyzwania. Od naszych cotygodniowych spotkań i zadań oczekuję ogromu praktycznej wiedzy, 
która pozwoli mi poczuć się jak w prawdziwym projekcie. Jestem zaciekawiona i z niecierpliwością będę wyczekiwać kolejnych tasków. :)
## Subtask 4
*1. Do czego służy aplikacja?*

   Aplikacja służy do gromadzenia informacji o graczach/piłkarzach. 
   Znajdziemy w niej szczegółowe informacje o konkretnym piłkarzu (pochodzenie, pozycja, cechy fizyczne). 
   Każdy gracz ma przypisaną historię meczy, w których grał oraz można sprawdzić sumaryczny raport z meczu.
   Raporty można uzupełniać o szczegółowe informacje dotyczące zachowania zawodnika na boisku.
    
*2. Jakie funkcjonalności ma aplikacja?*

   **W aplikacji można wyróżnić następujące funkcjonalności:**
   * Dodawanie gracza do listy; 
   
     *UWAGA: Opcja dodania gracza z widoku zakładki gracze, byłaby wygodna i intuicyjna.
      UWAGA: Możliwość edycji informacji o zawodniku, nie powinna być dostępna po naciśnięciu w konkretny wiersz (imię i nazwisko gracza), 
             uważam że powinna się wyświetlać strona, która jest podsumowaniem, a nie edycją. Opcja edycji mogłaby być dostępna tylko dla autora rekordu.*
   * Dodawanie i edcyja informacji o meczu, które są przypisane do określonego gracza;
   
     *UWAGA: Możliwość wejścia do zakładki "Mecze" z menu głównego, byłaby wygodna i intuicyjna.
             Ktoś może znać informacje z meczu i chcieć kogoś znaleźć, bez znajmości imienia i nazwiska gracza.*
   * Ściąganie listy graczy w postaci plików *.CSV;
   * Wydruk listy graczy, poprzez naciśnięcie odpowiedniej ikony;
   * Możliwość zmiany wyświetlanej tabeli z graczami (np. ukrywanie kolumn);
   * Filtrowanie listy graczy;
   
      *UWAGA: Powinna być dostępność podstawowych filtrów, czyli sortowanie alfabatyczne, rosnące, malejące (np. wiekiem, ilością meczy, raportów).*
   * Możliwość wyszukiwania zawodników.
    
*3. Interfejs aplikacji*

   Strona jest prosta, nie za bardzo rozbudowana. Na pierwszy rzut oka większość funkcji wydaje się intuicyjna. 

*4. Intuicyjność*

   Z poziomu strony głównej wszystko jest jasne. Występuje opcja "Dodaj gracza", widać które informacje odsyłają nas do kolejnych stron.
   Z poziomu zakładki "Gracze" brak możliwości dodania nowego gracza. Mogłaby pojawić się opcja dodania gracza w tym oknie.
   Na stronie głownej pojawiają się informacje o ilości gracze, maczy, raportów, jednak oprócz graczy nie możemy niczego innego przeglądać.
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
   
   * "Po dodaniu gracza przekierosuje nas na stronę edycji"
   
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
      
  * "W oknie dodawania gracza, przycisk "Clear" nie usuwa informacji z formulkarza."
      
      Rezultat: Po kliknięciu w przycisk "Clear" w formularzu edycji informacji o graczu, nie następuje usunięcie danych.
   
      Oczekiwany rezultat: Usunięcie danych w formularzu.
   
      Priorytet: średni
      
   * "Możliwość dodania gracza bez danych"
      
      Rezultat: Stworzenie konta gracza, po wpisaniu SPACJI w puste pola.
   
      Oczekiwany rezultat: Informacja o konieczności wypełnienia pustego pola ciągiem znaków, cyfr.
   
      Priorytet:wysoki 
      
   **Ogólny komentarz:**
   
      Sekcja dodawania graczy i wszystkie pola do uzupełnienia powinny być zablokowane przeed wpiasaniem niepoprawnych danych.
      Puste pola lub pola ze spacją, abstrakcyjne wartości wagi i wzorstu, blokada przed wpisaniem litery w pola numeryczne (numer telefonu).
      Brakuje profilu osoby zalogowanej, gdzie moglibyśmy sprawdzić ile osób dodaliśmy do bazy, gdzie widniałyby nasze dane.
