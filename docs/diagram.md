# 🗺️ Diagram Przepływu (Flowchart)

```mermaid
graph TD
    A[Start/Logowanie] --> B(Panel Główny/Pulpit);
    B --> C{Zarządzanie Zadaniem?};
    C -- Tak --> D[Lista Zadań: Dodaj/Edytuj];
    C -- Nie --> E{Przegląd Postępów?};
    E -- Kalendarz --> F[Widok Tygodniowy];
    E -- Statystyki --> G[Statystyki/Wykres Postępu];

    D --> H[Oznacz jako Wykonane];
    H --> B;

    F --> B;
    G --> B;

    B --> I[Wylogowanie/Koniec Sesji];