SkinAI to zaawansowany system oparty na sztucznej inteligencji, którego 
celem jest automatyczna analiza obrazów skóry w celu wykrycia i diagnozy 
różnych chorób skóry. Ma na celu zapewnienie szybkiej, dokładnej i metody 
diagnozowania chorób skóry, aby wesprzeć dermatologów i zwiększyć 
dostęp do wysokiej jakości opieki dermatologicznej. 


Język programowania: Python
Biblioteki: TensorFlow, Keras, NumPy, Matplotlib, scikit-learn
Funkcja: Klasyfikacja chorób skóry za pomocą sieci neuronowej konwolucyjnej (CNN)
Wejście: Zbiór danych obrazów skóry z etykietami
Wyjście: Ocena dokładności modelu, macierz pomyłek, raport klasyfikacji, wizualizacje dokładności i straty oraz przykładowe obrazy z przewidywaniami
Opis działania skryptu:

Ładowanie modelu: Skrypt rozpoczyna od wczytania wytrenowanych wag do modelu, które najlepiej sprawdziły się na danych walidacyjnych.

Ocena modelu: Model jest oceniany na zbiorze danych testowych, a wyniki (strata i dokładność) są wyświetlane na konsoli.

Predykcje: Wykonuje predykcje na zbiorze testowym, a następnie przypisuje najbardziej prawdopodobną klasę dla każdego obrazu testowego.

Prawdziwe etykiety: Skrypt przygotowuje wektor prawdziwych etykiet, używając danych z generatora testowego.

Wizualizacja historii treningu: Wyświetla wykresy dokładności i straty dla danych treningowych i walidacyjnych, co pomaga ocenić, jak model uczył się w czasie.

Macierz pomyłek: Tworzy i wyświetla macierz pomyłek, która jest graficznym przedstawieniem wyników klasyfikacji. Jest to użyteczne do zrozumienia, które klasy są mylone przez model.

Raport klasyfikacji: Skrypt generuje raport klasyfikacji, który zawiera metryki takie jak precyzja, pełność (recall) i wynik F1 dla każdej klasy.

Przykładowe przewidywania: Na końcu wyświetla pięć przykładów obrazów testowych wraz z ich prawdziwymi i przewidywanymi etykietami, co daje wgląd w działanie modelu.

Należy zwrócić uwagę, że powyższy skrypt musi być uruchomiony w środowisku, gdzie odpowiednie biblioteki są już zainstalowane i skonfigurowane, a także, że dane muszą być wcześniej przygotowane i podzielone na treningowe, walidacyjne i testowe. Skrypt zakłada także, że zbiór danych jest zbalansowany i odpowiednio oznakowany, a obrazy są przeskalowane do jednolitego rozmiaru.