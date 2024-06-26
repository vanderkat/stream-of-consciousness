{
   "categories": [
      "Soft"
   ],
   "date": "2022-03-31",
   "tags": [
      "EncFS",
      "Linux"
   ],
   "title": "EncFS GUI"
}

> EncFS — криптографическая файловая система, прозрачно шифрующая файлы, используя произвольный каталог в качестве места для хранения зашифрованных файлов.
> 
> Википедия

Очень удобная штука. Одна беда - у нее нет удобного графического интерфейса, а вводить каждый раз команду для подключения очень уж лениво.

Лениво это не только мне, поэтому - кто бы сомневался! - появилось множество графических оболочек, которые в красивом виде отображают шифрованные разделы, запрашивают пароль в красивых окошечках и сами выполняют команды для подключения.

**CryptKeeper** - компактная, удобная программка, которая выводит иконку в область системных уведомлений. Ничего лишнего - создать/импортировать шифрованный раздел, подключить/отключить его, запуститься при запуске системы. Она была бы идеальной, если бы не скандал с ошибкой, который позволял создавать разделы с универсальным паролем "p". Это ошибка была исправлена, но репутация программки пострадала настолько, что она была исключена из всех дистрибутивов Linux, а вскоре и вовсе заброшена автором.

**Gnome-encfs-manager** пришел ему на смену. Автор не скрывал, что вдохновлялись CryptKeeper-ом, поэтому возможности в этой программе были схожи, что называется, до степени смешения. И все бы хорошо, если бы на моем Mate под ArchLinux она не падала сразу после подключения зашифрованного раздела. Хотя Mate основан на том же самом GTK, что и Gnome, для которого это все и писалось.

**MEncfsM**. К счастью, Moritz Molch (автор gnome-encfs-manager) на своем [личном сайте](https://moritzmolch.com/) предлагает другую разновидность программы - статически скомпонованную с библиотеками Qt в один исполнимый файл, который даже не надо устанавливать в систему. Достаточно просто запустить - и все. На нем я и остановился.

На самом деле, есть еще много разных программ для того же самого (от компонентов KDE Plasma до совершенно наколенных скриптов на TCL/TK), но лучшее решение, сдается мне, я уже нашел.
