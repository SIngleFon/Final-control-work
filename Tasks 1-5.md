> 1. Используя команду cat в терминале операционной системы Linux, создать
два файла Домашние животные (заполнив файл собаками, кошками,
хомяками) и Вьючные животными заполнив файл Лошадьми, верблюдами и
ослы), а затем объединить их. Просмотреть содержимое созданного файла.
Переименовать файл, дав ему новое имя (Друзья человека).
>2. Создать директорию, переместить файл туда.
>3. Подключить дополнительный репозиторий MySQL. Установить любой пакет
из этого репозитория.
>4. Установить и удалить deb-пакет с помощью dpkg.
>5. Выложить историю команд в терминале ubuntu

1. 
cat >  Pets 

Собака Кошка Хомяк (ctrl + D)

cat > PackAnimals

Лошадь Верблюд Осёл (ctrl + D)

cat Pets PackAnimals > mrg

cat mrg 

mv mrg HumanFriends

2. 
mkdir test

mv HumanFriends test

3. 
sudo apt-get update

sudo apt install mysql-server

4.
wget https://dev.mysql.com/get/mysql-apt-config_0.8.26-1_all.deb

sudo dpkg --install mysql-apt-config_0.8.26-1_all.deb 

sudo dpkg -r mysql-apt-config


