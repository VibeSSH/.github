# VibeSSH

<p align="center">
  <a href="https://github.com/VibeSSH/.github/blob/main/profile/README.md">English</a> · <a href="https://github.com/VibeSSH/.github/blob/main/profile/README.pl.md">Polski</a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/VibeSSH/.github/main/profile/vibessh-dashboard.png"
       alt="Pulpit VibeSSH: dwa Node'y z bieżącym zużyciem procesora i pamięci oraz działające na nich aplikacje"
       width="880">
</p>

**Zarządzaj swoimi serwerami z Linuksem z aplikacji na komputerze. Nic do hostowania, żadnego panelu do utrzymywania.**

VibeSSH to aplikacja na Windowsa i Linuksa, która zarządza maszynami z
Linuksem po zwykłym SSH — i tym, co na nich faktycznie działa: serwerami
Minecrafta, bazami danych, botami. Instalujesz ją na własnym komputerze. Na
serwerze nie instalujesz nic, żeby zadziałała, i nie wystawiasz kolejnej
usługi w internecie tylko po to, żeby administrować jedną maszyną.

Bez domeny. Bez certyfikatu SSL. Bez nginxa. Bez hostowanego panelu.

## Co potrafi

**Serwery.** SSH z terminalem w kartach, przeglądarka plików po SFTP z
edytorem, bieżące metryki i procesy, akcje na systemd i Dockerze oraz
tymczasowe przekierowania portów.

**Aplikacje.** Serwer, baza danych albo bot prowadzone jako jedna całość, a
nie jako stos poleceń powłoki — uruchamiane, zatrzymywane, backupowane, z
własnymi plikami, portami, zmiennymi i logami. W komplecie czternaście
szablonów: Paper, Purpur, Velocity, Waterfall, MariaDB, MongoDB, Redis, NATS,
phpMyAdmin, boty w Node.js i Pythonie oraz uniwersalne na wszystko inne.
Działają jako kontenery Dockera, usługi systemd albo zwykłe procesy — również
na Twojej własnej maszynie, gdzie nie trzeba instalować niczego.

**Vibe Network.** Prywatna sieć WireGuard między Twoimi Node'ami, z nazwami
DNS dla aplikacji, dzięki czemu jeden serwer dosięga drugiego bez
publikowania portu do internetu.

**Firewall.** Reguły ufw wynikają z portów, które sam opublikowałeś — w tym z
ruchu kontenerów, którego samo ufw po cichu nie filtruje, co jest zwykłą
przyczyną tego, że „zamknięty" port jest otwarty.

**Kopie zapasowe.** Katalogi aplikacji, ręcznie albo według harmonogramu,
trzymane lokalnie i opcjonalnie wysyłane do S3, Cloudflare R2 lub MinIO.

**Migracja z Pterodactyla.** Serwery przenoszą się razem z plikami i
konfiguracją.

**Vibe AI.** Odpowiada na pytania o *Twoje* serwery, opierając się na
wbudowanym poradniku, przy użyciu klucza API, który sam podajesz.

## Skąd wziąć

Instalator dla Windowsa, AppImage, `.deb` i `.tar.gz`:
[**najnowsze wydanie**](https://github.com/VibeSSH/vibessh-releases/releases/latest)

Strona i dokumentacja: [**vibessh.dev**](https://vibessh.dev)

## Czy potrzebuję konta?

Nie. Node'y, aplikacje, pliki, terminal, firewall i kopie zapasowe działają
bez logowania się gdziekolwiek.

Konto służy wyłącznie do zespołów i współdzielonych serwerów. Jest hostowane
pod `api.vibessh.dev` i świeża instalacja wskazuje właśnie na nie, ale możesz
zamiast tego uruchomić backend u siebie — jest w repozytorium, a adres jest
ustawieniem.

Tak czy inaczej konto dotyczy dzielenia się serwerami z innymi ludźmi i
niczego więcej. Twoje dane logowania po SSH nie są jego częścią: hasła i
hasła do kluczy leżą w magazynie poświadczeń Twojego systemu operacyjnego, na
Twojej maszynie — nigdy w pliku konfiguracyjnym i nigdy na naszym serwerze.

## Status

Publiczna beta, wydawana regularnie. Kod źródłowy jest publiczny, na licencji
[AGPL-3.0](https://github.com/VibeSSH/vibessh/blob/main/LICENSE.txt) —
zgłoszenia i pull requesty są mile widziane w
[VibeSSH/vibessh](https://github.com/VibeSSH/vibessh).
