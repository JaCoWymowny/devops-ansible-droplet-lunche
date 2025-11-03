# Readme do repozytorium Git
Ten plik Readme opisuje działanie skryptu Ansible używanego do tworzenia serwera kroplekowego (Droplet) w Digital Ocean.

## Co robi ten skrypt?
Ten skrypt Ansible służy do tworzenia i zarządzania serwerami Droplet w Digital Ocean. Kiedy uruchomisz ten skrypt, stworzy on serwery Droplet z podanymi specyfikacjami, wyświetli ich adresy IP, odczeka na dostępność portu SSH (22) na tych serwerach, a następnie wygeneruje plik inwentarza yaml na podstawie szablonu.

## Zdefiniowane są cztery różne zadania:
1. TASK: {{ do_state }} mutiple droplet - to zadanie tworzy serwery Droplet na podstawie podanych specyfikacji.
2. TASK: Display IP addresses - to zadanie wyświetla adresy IP utworzonych serwerów Droplet.
3. TASK: Wait for port 22 - to zadanie oczekuje na dostępność portu 22 (SSH) na utworzonych serwerach Droplet.
4. TASK: Generate template yaml inventory - to zadanie generuje plik inwentarza yaml na podstawie szablonu.

## Wymagania
Aby użyć tego skryptu, musisz mieć:

- Konto na Digital Ocean
- Token API Digital Ocean
- Zainstalowane Ansible na swoim komputerze

## Jak go używać?
1. Sklonuj to repozytorium na swój lokalny komputer.
2. Otwórz plik skryptu Ansible.
3. Zastąp "{{ do_api_token }}" swoim tokenem API Digital Ocean.
4. Możesz dostosować nazwę droplet, region, obraz, rozmiar, projekt i klucze ssh według swoich potrzeb.
5. Uruchom skrypt Ansible, używając polecenia ansible-playbook `<nazwa_pliku>.yml`

Uwaga: Używanie tego skryptu pociąga za sobą opłaty związane z używaniem serwisów Digital Ocean. Pamiętaj, aby usunąć wszelkie zasoby, których nie potrzebujesz, aby uniknąć niepotrzebnych kosztów.

## Wsparcie
Jeśli masz jakiekolwiek pytania lub problemy związane z tym skryptem, utwórz nowy problem w tym repozytorium.

## Licencja
Ten projekt jest licencjonowany na podstawie licencji MIT.

## Potrzebujesz wsparcia masz pytania zapraszam do grupy:
- [Discord](http://discord.helppointit.cloud) (http://discord.helppointit.cloud)
- [Grupa Facebook](http://facebook.helppointit.cloud) (http://facebook.helppointit.cloud)

## Szukasz innych szkoleń?

Zapraszam na naszą platformę [Szkolenia Cloud](https://szkolenia.cloud) Znajdziesz tu różnego rodzaju szkolenia.

## Teraform
Jest to kurs z podstaw terraform - nauczysz sie i poznasz narzedzie terraform na praktycznych przykładach. [Link do kursu](https://szkolenia.cloud/product/terraform-podstawy/)
[![Kurs Terraform](https://cdn.idealms.net/5061/edd/MiniaturaKursuTerraformPodstawy.png)](https://szkolenia.cloud/product/terraform-podstawy/)

## Docker
Kurs na temat konteneryzacji - praktyczne przykłady, konfiguracja środowiska produkcyjnego. [Link do kursu](https://dockerakademia.pl/)
[![Kurs Docker](https://cdn.idealms.net/5061/333991.jpg)](https://dockerakademia.pl/)

## Inne materiały do których warto zajrzeć:
W kursie jest poruszanych kilka tematów - które oczywiście nie mogły być rozwiniete szczegołowo, zatem jeżeli chcesz pogłebić wiedzę z danego tematu zapraszam do odpowiednich kursów:
1. Kurs z tematyki [Ansible](https://strefakursow.pl/kursy/programowanie/kurs_ansible_-_automatyzacja_zadan_w_praktyce.html?ref=52966)


2. Temat związany z konteneryzacją poziom zaawansowny - [Kurs Docker](https://strefakursow.pl/kursy/programowanie/kurs_docker_dla_zaawansowanych.html?ref=52966)

3. Teamty sieciowe w systemach linux - [Kurs Konfiguracji sieci](https://strefakursow.pl/kursy/it_i_oprogramowanie/kurs_podstawy_networkingu_oraz_konfiguracji_sieci_w_linux.html?ref=52966)

4. Rozwiniecie tematu konfiguracji [Nginx](https://strefakursow.pl/kursy/it_i_oprogramowanie/kurs_nginx_-_wydajne_serwery_od_podstaw.html?ref=52966)

5. Tematyka związana z Systemem Kontroli Wersji - [Git poziom zaawansowany](https://strefakursow.pl/kursy/programowanie/kurs_git_dla_zaawansowanych.html?ref=52966)

6. System Kontroli Wersji - [Kurs Git dla poczatkujących](https://strefakursow.pl/kursy/programowanie/kurs_git_dla_poczatkujacych.html?ref=52966)

7. Jezeli sprawia Ci poruszanie się po edytorze vim zapraszam do [Kursu Vim podstawy](https://strefakursow.pl/kursy/programowanie/kurs_vim_-_techniki_pracy.html?ref=52966)

8. Administracja Serwerem [Linux - Kurs dla średniozaawansowanych](https://strefakursow.pl/kursy/it_i_oprogramowanie/administracja_serwerem_linux.html?ref=52966)

9. Administracja Serwerem [Linux - Kurs dla zaawansowanych](https://strefakursow.pl/kursy/it_i_oprogramowanie/zaawansowana_administracja_systemem_linux.html?ref=52966)

10. Kurs [Linux dla osób poczatkujących](https://strefakursow.pl/kursy/it_i_oprogramowanie/kurs_linux_dla_poczatkujacych.html?ref=52966)

11. Trochę o automatyzacji z wykorzystaniem Bash - [Kurs o skryptach i automatyzacji w Bash](https://strefakursow.pl/kursy/programowanie/kurs_bash_-_skrypty_i_automatyzacja.html?ref=52966)