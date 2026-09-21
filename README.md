# Centurion Desktop — releases

Installers and the auto-update feed for the **Centurion desktop client (C#/WPF)**.
The Electron client ships separately from [centurion-releases](https://github.com/PeterSmithski/centurion-releases).

## Instalacja

1. Otwórz najnowsze wydanie w zakładce **Releases**.
2. Pobierz `CenturionDesktop-win-Setup.exe` i uruchom go.
   Windows może pokazać „System Windows ochronił ten komputer” — kliknij
   **Więcej informacji → Uruchom mimo to** (instalator nie jest podpisany cyfrowo).
3. Program instaluje się dla bieżącego użytkownika (bez uprawnień administratora) i sam się
   aktualizuje: sprawdza nowe wersje przy starcie, co cztery godziny oraz po kliknięciu
   „Sprawdź aktualizacje”.

Obraz z rejestratorów Hikvision wymaga pakietów Microsoft Visual C++ Redistributable
2008 SP1 (x64) i 2013 (x64): https://learn.microsoft.com/cpp/windows/latest-supported-vc-redist

---

Releases are published automatically by the `release-desktop.yml` workflow in the main
repository on a `desktop-vX.Y.Z` tag. Do not upload or edit assets here by hand —
`releases.win.json` is what installed clients read.
