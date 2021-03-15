# Szablon pracy dyplomowej na UPH

Te repozytorium zawiera szablon latex pracy dyplomowej zgodnej z zasadami Uniwersytetu Przyrodniczo-Humanistycznego.

# Quickstart

1. Otwórz plik *oswiadczenie_i_tytulowa.odt* i podmień temat pracy, imię *"Jan Kowalski"* na swoje oraz imię *"Mateusz Nowak"* na imię twojego promotora.
2. Wyeksportuj ten plik do pdf o nazwie `oswiadczenie_i_tytulowa.pdf`.
3. Przejdź do folderu chapters i podmień słowa kluczowe oraz tytuł pracy w pliku `0_slowa_kluczowe.tex`
4. Następnie utwórz dla każdego rozdziału w tym folderze plik .tex o takim formacie `3_nazwa_rozdzialu.tex` gdzie 2 będzie numerem rozdziału a `nazwa_rozdzialu` nazwą rozdziału. Ta konwencja
nazewnicza nie jest konieczna ale łatwiej potem się połapać, który rozdział jest którym.
5. Ostatnim krokiem jest cofnięcie się do folderu wyżej, otworzenie pliku main.tex i następnie w okolicy linijki 65 dla każdego rozdziału zamieścić poniższy skrawek kodu:

```
\chapter{Nazwa rozdziału}
\input{Chapters/3_nazwa_rozdzialu.tex}
```

Nazwy rozdziału oraz nazwa pliku oczywiście musi być adekwatna do wcześniej utworzonych plików rozdziałów.

Et voilà ! Wystarczy skompilować projekt i masz rozkład swojej pracy dyplomowej. Plików wstępu oraz podsumowania nie musisz tworzyć - jest już on utworzony w `Chapters/1_wstep.tex` oraz `Chapters/podsumowanie.tex`. Wystarczy go zapełnić. Bibliografię wrzucaj do `References.bib`. Jeżeli chcesz wiedzieć jak szybko załączać grafikę, wzory, dodawać tablice oraz skrawki kodu to zerknij to pliku `2_rozdzial_pomoc.tex` w folderze chapters. 

# Problemy

Jeżeli napotkasz jakieś problemy z tym szablonem to załóż proszę issue na tym repozytorium bądź jak masz chęci naprawy go to utwórz pull requesta z fixem a przejrzę go w wolnym czasie.
 
