# SkinAI
1.	Charakterystyka oprogramowania: 

a) krótka nazwa: SkinAI 
b) pełna nazwa: System sztucznej inteligencji do wykrywania chorób skóry 
c) krótki opis z przeznaczeniem: 

•	SkinAI to zaawansowany system oparty na sztucznej inteligencji, którego celem jest automatyczna analiza obrazów skóry w celu wykrycia i diagnozy różnych chorób skóry. Ma na celu zapewnienie szybkiej, dokładnej i metody diagnozowania chorób skóry, aby wesprzeć dermatologów i zwiększyć dostęp do wysokiej jakości opieki dermatologicznej. 

•	Analizuje obrazy skóry, takie jak zdjęcia, skanowanie dermoskopowe, a nawet zdalne obrazy przesłane przez pacjentów, w celu rozpoznania różnych schorzeń skórnych. Może rozpoznać powszechne choroby, takie jak trądzik, łuszczyca, egzemy, znamiona skórne, a także bardziej poważne schorzenia, takie jak czerniak czy raki skóry. Właściwa klasyfikacja chorób skóry przez system SI pozwala również na szybsze wdrożenie odpowiedniego leczenia.

•	Dzięki wykorzystaniu technik uczenia maszynowego, system SI może przetwarzać duże ilości danych w krótkim czasie, co przyspiesza proces diagnozy i eliminuje opóźnienia wynikające z konieczności oczekiwania na wizytę u lekarza. System SI jest ciągle rozwijany dzięki ciągłemu doskonaleniu i aktualizacji swojego algorytmu na podstawie nowych danych i informacji zwrotnych od lekarzy. W miarę gromadzenia większej liczby przypadków schorzeń skórnych, system SI staje się coraz bardziej precyzyjny i dokładny w swoich diagnozach. 


2.	Prawa autorskie: 

a) autorzy: AI Medical Zaspa
b) warunki licencji: MIT
•	Licencja MIT to otwarta licencja oprogramowania, która umożliwia osobom, które otrzymują oprogramowanie, jego używanie w dowolnym celu, zarówno komercyjnym, jak i niekomercyjnym, bez żadnych ograniczeń
3.	Specyfikacja wymagań: 
Identyfikator	Nazwa	Opis	Priorytet	Kategoria
REQ001	Analiza obrazu skóry	System powinien przetwarzać obrazy skóry w celu wykrycia chorób	1
(wymagane)	Funkcjonalne




REQ002	Klasyfikacja chorób skórnych	System powinien klasyfikować zidentyfikowane choroby skórne	1	Funkcjonalne

REQ003	Interfejs użytkownika	System powinien posiadać intuicyjny interfejs użytkownika	2
(przydatne)	Funkcjonalne
REQ004	Wydajność systemu	System powinien przetwarzać obrazy skóry w czasie rzeczywistym	1	Pozafunkcjonalne
REQ005	Bezpieczeństwo danych	System powinien zapewniać bezpieczne przechowywanie danych	1	Pozafunkcjonalne
REQ006	Skalowalność	System powinien być skalowany, aby obsłużyć wzrost liczby pacjentów	2
	Pozafunkcjonalne
REQ007	Dostępność	System powinien być dostępny 24/7	2	Pozafunkcjonalne
REQ008	Dokładność diagnoz 	System powinien osiągać wysoki poziom dokładności diagnoz	1	Pozafunkcjonalne
REQ009	Monitoring systemu	System powinien umożliwiać monitorowanie działania i wydajności	1	Pozafunkcjonalne
REQ010	Współpraca z innymi systemami	System powinien integrować się z istniejącymi systemami medycznymi	3
(opcjonalne)	Pozafunkcjonalne


4.	Architektura oprogramowania 

Architektura rozwoju - stos technologiczny:
•	Język programowania: Python
•	Framework do tworzenia interfejsu użytkownika: Django
•	Biblioteka do analizy obrazów: OpenCV
•	Biblioteka do uczenia maszynowego: TensorFlow
•	Baza danych: PostgreSQL
•	Narzędzie do wersjonowania kodu: Git
•	Środowisko wirtualne: Anaconda
•	System kontroli zależności: pip
•	Narzędzia do testowania: pytest, Selenium
•	Narzędzie do zarządzania projektem: Jira

Architektura uruchomieniowa - stos technologiczny:

•	Serwer aplikacyjny: Gunicorn
•	Serwer HTTP: Nginx
•	System operacyjny: Linux
•	Chmura obliczeniowa: Amazon Web Services (AWS) lub Microsoft Azure
•	Monitorowanie: Nagios, Prometheus
•	Logowanie i analiza dzienników: ELK Stack (Elasticsearch, Logstash, Kibana)
•	Konteneryzacja: Docker
•	Orkiestracja kontenerów: Kubernetes
•	Skalowalność i równoważenie obciążenia: Kubernetes Autoscaling
•	Zabezpieczenia: Firewall, SSL/TLS

5.	Testy: 

1.	Dla REQ001 - Analiza obrazu skóry:

•	Przesłanie obrazu zdrowej skóry do systemu w celu analizy
•	Przesłanie obrazu z widocznymi zmianami skórnymi

2.	Dla REQ002 - Klasyfikacja chorób skórnych:

•	Przesłanie obrazu z objawami choroby skóry do systemu
•	Identyfikowanie choroby i klasyfikowanie

3.	Dla REQ002 – Interfejs użytkownika:

•	Przesłanie obrazu skóry za pomocą interfejsu użytkownika
•	Przeglądanie wyników analizy skóry
•	Wyświetlanie zaleceń i porad dotyczących zdrowia skóry

4.	Dla REQ004 - Wydajność systemu:

•	Przetwarzanie obrazu w czasie 
•	Przesłanie obrazu skóry o średniej wielkości do systemu w celu przetestowania jego wydajności w czasie rzeczywistym

5.	Dla REQ005 – Bezpieczeństwo danych:

•	Sprawdzenie czy system zapewnia bezpieczne przechowywanie danych pacjentów
•	Test dostępu nieautoryzowanego – Przesłanie danych do systemu i sprawdzenie, czy są one w zaszyfrowanej formie
•	Test szyfrowania danych - Przesłanie danych do systemu i sprawdzenie, czy są one przechowywane w zaszyfrowanej formie
•	Test zabezpieczeń sieciowych – Próba przejęcia danych w trakcie przysyłania przez sieć
•	Test zarządzania uprawnieniami użytkowników – Próba przechwycenia danych po przez złośliwe oprogramowanie

6.	Dla REQ006 - Skalowalność:

•	Przesłanie dużej liczby żądań do systemu w celu zbadania jego skalowalności (przyjęcie większej ilości użytkowników)


7.	Dla REQ007 – Dostępność:

•	Wysłanie żądania do systemu i pomiar czasu, jaki zajmuje mu udzielenie odpowiedzi
•	Sprawdzenie, czy system jest dostępny dla użytkowników przez całą dobę, 7 dni w tygodniu.

8.	Dla REQ008 – Dokładność diagnoz:

•	Porównanie diagnozy systemu z diagnozą eksperta dermatologa
•	Przesłanie obrazu zidentyfikowanej choroby do systemu i porównanie diagnozy systemu z diagnozą eksperta

9.	Dla REQ009 - Monitoring systemu:

•	Sprawdzenie, czy system umożliwia monitorowanie jego działania i wydajności
•	Monitorowanie dostępności systemu i rejestrowanie czasu przestoju w celu śledzenia i analizy czasu niedostępności


10.	Dla REQ010 – Współpraca z innymi systemami:

•	Wysłanie żądania do systemu w celu sprawdzenia poprawności integracji z system z bazą danych (odczytanie i zapisywanie danych)
•	Próba logowania się do systemu przy użyciu danych z systemu zarządzania użytkownikami np. za pomocą konta Google lub Facebook
•	Przesłanie plików do systemu lub pobranie plików z systemu w celu sprawdzenia integracji z systemem zarządzania plikami np. usługi chmurowej



