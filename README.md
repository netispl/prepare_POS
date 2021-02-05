
## Informacje
Playbook do konfiguracji POS'a przygotowanego przez NETIS.

## Wymagania
Komputer musi być mieć zainstalowany wzór POS'a **Ubuntu 18 64 bit**

## Wymagane pakiety

 ```
 sudo apt-add-repository multiverse
 sudo apt-add-repository --yes ppa:ansible/ansible
 sudo apt-get install --yes --force-yes git ansible
 ansible-galaxy collection install community.mysql
```

## Instalacja
Uruchomienie playbooka - (wymaga podania hasła do odszyfrowania klucza):
```
 sudo ansible-pull -U https://github.com/netispl/prepare_POS -i hosts
```
