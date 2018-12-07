---
layout: post
title:  "Używalność Core2Duo w 2018 roku"
tags:
  - Dell
  - Latitude
  - E6500
  - Core2Duo
  - C2D
  - Centrino vPro
hero: uploads/latitude-e6500.jpg
overlay: blue
published: true

---
<!–-break-–>

## Awaria płyty głównej zmusiła mnie do przesiadki na **Della Latitude E6500**
### Na początek chciałbym przedstawić specyfikację laptopa, z którego obecnie korzystam:
- **CPU:** Intel Core2Duo P8700
- **GPU:** nVidia Quadro NVS 160M
- **RAM:** 4GB
- **SSD:** Adata SU800 128GB

Niestety, z racji tego że laptop za 2 tygodnie musi wrócić do właściciela nie mogę postawić tutaj **GNU/Linuxa**, ale dostałem zgodę
na zrobienie formata, to też uczyniłem.

## Jaki system wybrać na 10 letni komputer, gdy w grę wchodzą tylko systemy Microsoftu?
Wybór padł na *64-bitowego* **Windowsa 10 Education 1809**. Z początku system nie działał zbyt dobrze, lecz jego konfiguracja zdecydowanie
polepszyła ten stan rzeczy. Poniżej postaram się streścić, co dokładnie uczyniłem.

### Konfiguracja systemu Windows 10
- Wyłączenie zbędnych usług (```services.msc```)
- Wyłączenie **Microsoft Store** (```gpedit.msc```)
- Ustawienie swap file na 4GB
- Usunięcie zbędnych aplikacji UWP

Te podstawowe kroki sprawiły, że system *"na dzień dobry"*
używa jedynie 1GB RAMu, oraz znacząco obniżył użycie
procesora *(głównym winowajcą był Microsoft Store)*. Sam system
znaczaco przyspieszył, i nawet dla mnie jest całkiem używalny.

## Do czego nadaje się ten laptop?
- **Proste programowanie**, mój ulubiony edytor kodu - **Visual Studio Code**
działa na prawdę przyjemnie, nie ma problemów z freezami czy dużym
opóźnieniem pomiędzy naciśnięciem przycisku na klawiaturze a wprowadzeniem go do pliku,
mimo, że laptop ma na prawdę bardzo przyjemną klawiaturę,
i piszę na niej nie wiele wolniej od tego, co pisałem na codzien
korzystając z mojej stacjonarki. Co prawda czas kompilacji pozostawia,
trochę do życzenia, jeśli nie mamy zamiaru kompilować na tym mega
zaawansowanych projektów, to laptop ten powinien dać sobie radę.

- **Surfowanie po sieci** nie sprawia laptopowi żadnych problemów.
Jestem przyzwyczajony do pracy przy 15-20 kartach w przeglądarce, i
początkowo obawiałem się, że z tym osiągnięcie chociaż zbliżonego wyniku będzie awykonalne. Myliłem się, przy 5-10 działających kartach
gdy jedna z nich to YouTube z działającą muzyką w 144p surfowanie
jest całkiem przyjemne. Obstawiam że to zasługa dysku SSD i
działającego na nim swapu. Na tym laptopie korzystam z Opery, nie wiem
jak by to wyglądało gdybym korzystał z ulubionego chromium.

- **Oglądanie filmów** w serwisie YouTube w rozdzielczości 1080p
nie sprawia temu laptopowi problemów, a sam ekran ma rozdzielczość 1440x900 *(16:10)*.

- **Granie w proste gry**. Nie jestem jakimś zahardowanym graczem,
lubię sobie od czasu do czasu pograć w [PokeMMO](https://pokemmo.eu/).
Podczas kilku godzin spędzonych w tej grze framerate ani razu nie spadł
poniżej 60fps. Za jakiś czas możliwę że zedytuję ten wpis, i podzielę
się wrażeniami z grania w [League Of Legends](https://eune.leagueoflegends.com)
na tym laptopie.

## Czy jest coś, w czym ten laptop sprawuje się lepiej niż współczesne sprzęty?
Owszem, jest to laptop stricte biznesowy, podobnie jak seria **ThinkPad** od **IBM/Lenovo**. Laptopy biznesowe charakteryzują się
dobrą jakością wykonania, obcując z tym urządzeniem nie mam wrażenia,
że zaraz się rozleci, tak jak to jest z **Lenovo IdeaPadem Z500** mojej mamy.

### Przewaga laptopów biznesowych **(W tym opisywany E6500)** względem laptopów konsumenckich.
- O niebo lepsza jakość wykonania,
- Zazwyczaj karta graficzna z serii **Quadro** lub **FirePro/Radeon Pro**
- Lepszy czas pracy na baterii *(W przpadku nowego laptopa oczywiście)*
- Lepszy serwis gwarancyjny
- Bajery typu:
    - **TPM**
    - **Czytnik linii papilarnych**
- Ilość portów - nie ciężko znaleźć w takich laptopach złącza **FireWire**, **eSATA**, **Mini-Jack 3.5mm** czy **USB-A**.
- Mnogość ustawien w **BIOS/UEFI**, na przykład:
    - Harmogram włączania/wyłączania laptopa
    - Automatyczne włączenie laptopa po podłączeniu zasilacza
    - Wyłączenie technologii **Nvidia Optimus**
    - Opcja ustawienia limitu naładowania baterii
    - Wiele innych

- Wsparcie społeczności **TYCZY SIĘ GŁÓWNIE THINKPADÓW**
    - Customowe BIOSy umożliwiające zdjęcie whitelisty WiFi
    - Dostępność [CoreBoota](https://www.coreboot.org)
    - Poradniki do hardwarowych modów na przykład:
        - wymiana matrycy na tą z wyższego modelu
        - wymiana klawiatury
- Łatwy dostęp do podzespołów

## Czy z takiego laptopa da się w dzisiejszych czasach korzystać?

Jak najbardziej tak, jeśli nie zamierzacie na nim grać, bawić się w maszyny wirtualne, grafikę czy kompilowanie kerneli, to laptop
powinien wam ładnie służyć. Świetny wybór jako prezent dla waszych
rodziców czy dziadków. Taki laptop wraz z dyskiem SSD zapewni komfort pracy przy przeglądaniu internetu.