---
layout: post
title:  "Dlaczego fanbase Windowsa jest zły oraz krótkie porównanie dwóch systemów."
tags:
  - GNU
  - GNU/Linux
  - Linux
  - Windows
  - FOSS
hero: uploads/linusnvidia.png
overlay: blue
published: true

---
<!–-break-–>
# Udzielając się na wielu grupach na fejsbuku wszyscy mówią, że Windows jest najlepszy, bo oni z niego korzystają.
Niestety, ciężko jest znaleźć użytkownika **Windowsa**, który ma jakiekolwiek pojęcie nt wszelkiej maści systemów operacyjnych.
Często ich jedynym argumentem jest: *Pograj se na linuxie* czy *Ja tam wolę korzystać z systemu który działa bez kompilowania jądra 2137 razy*.
Ludzie nadal nie dostrzegli postępu, jaki zrobił **GNU/Linux** przez ostatnie lata. To już nie jest ten system, który musisz instalować spod
CLI, i kompilować na nowo jądro żeby ściszyć/podgłośnić dźwięk. Mamy na rynku tyle dobrych a zarazem user-friendly dystrybucji, że nie ciężko pokusić
się o stwierdzenie, że **GNU/Linux** jest łatwiejszy **Windowsa** (patrz: **Fedora** czy **OpenSUSE**). Przejrzysty graficzny instalator, przejrzysta
dokumentacja i brak wypierdolki co każdy update (chyba że jesteś Windows Insiderem, tam wszystko działa lepiej niż na stable-branchu XD). Dodatkowo
warto wspomnieć o projekcie [FlatPak](https://flatpak.org), czyli nowej metodzie dystrybuowania oprogramowania, dzięki której nie musimy siedzieć
przed komputerem 2 dni rozwiązując 2137 zaleności i konfliktów dla aplikacji którą chcemy zainstalować.
Często zadając ludziom podstawowe pytania typu: *Jak nazywa się format binarek Windowsych* czy *Co to jest MBR* jako odpowiedź słyszymy
*Mam Windowsa, chuj mnie to obchodzi, ważne że działa*. Czy ludzie którzy sami się przyznają do tego, że nie mają kompletnie żadnej
wiedzy na temat tychże systemów powinni się na ich temat wypowiadać? Moim zdaniem *nie*.

## Zalety i wady Windowsa:
Zalety:
  * Dostępność oprogramowania *(To co mnie trzyma zdala od GNU/Linuxa)*
  * Smaczki których nie ma żadne GNU/Linuxowe DE typu: historia schowka, timeline, dopracowany screenshooter, Windows Hello \

Wady:
  * System plików, dzięki któremu nasz system aktualizuje się czasem nawet kilka godzin, i potrzebuje przy tym reboota.
  * Stabilność, a raczej jej brak. Kolejny feature update to kolejne problemy. Nieironicznie mówię, że problemy które
    pojawiają się przy feature updatach nie występują w programie Insider.
  * Totalny brak rozwoju. Micro$oft skupił się na poprawie UX, czyli tym co widzą zwykli Kowalscy. Zamiast poprawiać kernel
    wolą dodawać kolejne wodotryski typu: *Fluent Design* czy *Dark Theme*. Nie twierdzę że te zmiany są zbędne, jednak
    patrząc na rozwój sceny Linuksowej widać większy progres. Co kolejne wydanie [mesy](https://www.mesa3d.org), [amdgpu](https://en.wikipedia.org/wiki/AMDGPU)
    czy też samego [kernela](https://kernel.org/) dostajemy poprawę wydajności, stabilności i nowe funkcje.
  * Duża ilość bloatware-u. Wraz z czystą instalacją Windowsa dostajemy: *Minecrafta*, *Aplikację XBOX* i masę innego gówna. Domyślnie
    włączona jest ogromna ilość zbędnych usług systemowych, wyłączenie ich powoduje zmniejszenie użycia RAMu nawet o 1GB.
  
## Zalety i wady GNU/Linuxa:
Zalety:
  * szybki rozwój o którym wspomniałem omawiając wady systemu Micro$oftu.
  * Moc community. Z racji tego, że GNU/Linux jest systemem open-source, każdy może dołożyć swoją cegiełkę do jego rozwoju. Dzięki temu
    mamy takie projekty jak np. [wine](https://winehq.org) czy [vfio](https://wiki.archlinux.org/index.php/PCI_passthrough_via_OVMF) dzięki
    którym możemy uruchomić nasze ulubione gry na GNU/Linuksie. Przy okazji wine warto wspomnieć o chociażby [dxvk](https://github.com/doitsujin/dxvk)
    czyli wraperze **DirectX 11 -> Vulkan** lub ***Galium Nine*** czyli natywnej implementacji **DirectX 9** która pozwoli nam grać w Windowsowe gry 
    z jeszcze większą wydajnością niż natywnie na Windowsie. Wszystkie FOSS projekty związane z GNU/Linuxem mógłbym wymieniać tu do rana.
  * Stabilność i [wydajność](https://www.phoronix.com/scan.php?page=article&item=2990wx-linux-windows&num=1). GNU/Linux nie wypierdala się co update 
    *(Chyba że masz kartę novideo, to wtedy tak XD)*, ani nie zwalnia znacząco po jednym dniu uptime' u.
  * Updaty bez rebootów trwających 2137h \
  
Wady:
  * Mniejsza dostępność oprogramowania *(To właśnie mnie trzyma z dala od tego systemu)*
  * Częste zaniedbanie użytkowników tego systemu przez producentów sprzętu. O dobry przykład nie trzeba iść daleko,
    wystarczy spojrzeć na *nvidie*, która na twórców tego systemu ma totalnie wyjebane. Owszem, wypuszczają sterowniki na ten system
    jednak pozostawiają one wiele do życzenia, problemy z Waylandem, częste problemy przy aktualizacji kernela to codzienność. Gdyby jeszcze nvidia, poszła
    śladem AMD, i wypuściła ładną dokumentację, zamiast dostarczania [blobów](https://en.wikipedia.org/wiki/Binary_blob) które twórcy *nouveau* (otwartych sterowników)
    muszą reversować, co znaczaco utrudnia stworzenie dobrych sterowników, to tego problemu by nie było. Wolne sterowniki do kart AMD *(amdgpu)* są często
    lepsze od ich zamkniętej alternatywy *(AMDGPU-Pro)*, a przy okazji nie sprawiają problemów co aktualizację jądra, i ładnie współpracują z waylandem.
    Otwartoźródłowe sterowniki rozwijają sami pracownicy **zaawansowanych mikrourządzeń**.

## A więc który system powinienem wybrać?
Myślę że warto samemu spróbować. Nawet jeśli ten system nie przypadnie Ci do gustu, będzie to świetny eksperyment. Na **GNU/Linuxie** można grać dzięki
[wine](https://winehq.com) i [dxvk](https://github.com/doitsujin/dxvk) jednak jest to dosyć czasochłonne. Jeśli chcesz prostego rozwiązania możesz 
wypróbować *Protona* wbudowanego w platformę *Steam*. Jeśli korzystasz z innego specjalistycznego software' u *(W moim przypadku jest to pakiet od Adobe)*
to masz problem. Ten software nie działa dobrze przez *wine*. Wtedy zostań na Windowsie lub zainteresuj się tematem [Hackintosha]("https://hackintosh-polska.pl)
czyli instalacji systemu macOS na zwykłym komputerze PC.