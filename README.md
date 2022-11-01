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
             uważam że powinna się wyświetlać strona, która jest podsumowaniem, a nie edycją.*
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

   Strona jest prosta, nie za bardzo rozbudowana. Na pierwszy rzut oka

*4. Intuicyjność*

*5. Błędy*

   * "Niepoprawne ściąganie listy graczy w postaci pliku *.CSV"
    Środowisko: Windows 10, Chrome Wersja 107.0.5304.88
    Rezultat: Ściągnięcie listy graczy tylko z aktualnie otwartej strony spisu zawodników (10 rekordów).
    Oczekiwany rezultat: Ściągnięcie całej bazy zawodników.
    Kroki: 
      1. Otwórz stronę: https://scouts-test.futbolkolektyw.pl/pl 
      2. Zaloguj się poprawnymn loginem i hasłem.
      3. Otwórz zakładkę "Gracze" z bocznego menu.
      4. Pobierzlistę graczy *.CSV, klikacjąc ikonę chmury.
    Priorytet: niski
    *Komentarz: Mam na uwadzę sytuację, że taka funkcjonalność mogła zostać tak zaprojektowana, 
               jednak ze względu na użyteczność wydaje mi się, że wygenerowanie raportu z listą dostępnych graczy w całości,
               byłoby bardziej optymalne (przeniesienie do innej aplikacji/bazy).*
   * "W sekcji "Gracze" po najechaniu na zawodnika nie wyświetla się odsyłacz do indywidyulanej strony"
    Rezultat: Najechanie na wiersz z graczem nie wskazuje na możliwość kliknięcia.
    Oczekiwany rezultat: Pojawienie się odsyłacza do indywidualnej strony zawodnika.
    Priorytet: niski
   * 
