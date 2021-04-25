"Program do przechowywania obrazów"

FORK repozytorium
 2. Zbuduwalem aplikację w Dockerze i wypchnął ją do DockerHub na swoje konto.
 3. Uruchomil serwer A z ubuntu, który jest na porcie 80 i ma docker zainstaliowany
 4. Stworzylem  w repozytorium gitlab-ci pipeline. 
 5. Pipeline odbudowuje aplikację z repozytorium, gdy nastąpe zmiany w folderze  APP, później wysylam nowy obraz do docker hub, zeby  połączyć się z serwerem A przez OPEN-SSH.
 6. Zainstalowalem nową wersję obrazu docker na ten serwer, i uruchomilem kontener send, na porcie 80.

