## Array-Funktionen

`.map()` funktioniert mit Arrays

    [1, 2, 3].map((item) => item + 1);

    → [2, 3, 4]

UND Observables

    [1...2...3].map((item) => item + 1);

Nur eben auf einer Zeitleiste:

    → 2
    → 3
    → 4
