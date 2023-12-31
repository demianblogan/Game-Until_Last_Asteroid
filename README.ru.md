[![en](https://img.shields.io/badge/Language-English-red.svg)](https://github.com/demianblogan/Game-Until_Last_Asteroid/blob/main/README.md)
[![ru](https://img.shields.io/badge/Language-Russian-blue.svg)](https://github.com/demianblogan/Game-Until_Last_Asteroid/blob/main/README.ru.md)
[![ua](https://img.shields.io/badge/Language-Ukrainian-green.svg)](https://github.com/demianblogan/Game-Until_Last_Asteroid/blob/main/README.ua.md)

# Краткое описание игры
Это моя первая игра для моего портфолио. Её жанр "Shoot 'Em Up". В этой игре вы управляете космическим кораблем и стреляете по противникам, таким как астероиды и другие корабли. У вас есть несколько жизней, вы зарабатываете очки и проходите уровни.

![1](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/3b0eb5bc-6564-49be-a4cb-a588289da779)

## **Кнопки управления:**<br />
Arrow up    -> Двигаться вперёд<br />
Arrow left  -> Повернуть налево<br />
Arrow right -> Повернуть направо<br />
Arrow down  -> Прыгнуть в гиперпространство (прыгнуть в случайное место)<br />
Space       -> Стрелять<br />
Escape      -> Закрыть игру<br />

## **Как играть?**<br />
Когда вы запустите игру, вы увидите текст «Press any key to start». Это меню паузы. Каждый раз, когда вы умираете - вы будете видеть это окно. Если вы хотите закрыть игру в любое время - просто нажмите клавишу Escape. В игре бесконечное количество уровней. Каждый уровень содержит определенное количество астероидов и кораблей. Чтобы пройти уровень, вы должны уничтожить их всех и подождать, пока не исчезнут все ваши пули. (Каждая пуля исчезает через 5 секунд). В игре есть свой счет. Вы получаете очки за каждый уничтоженный астероид или корабль. За каждые 1000 очков вы получаете дополнительную жизнь. В начале игры у вас есть 3 жизни. Вы теряете одну жизнь, когда вас касается астероид, вражеский корабль или его пули. Если вы потеряете все свои жизни - игра перезапустится. Мир игры не имеет границ, поэтому если вы вылетели за одну сторону мира - окажетесь на другой его стороне.

## **Кто противники?**<br />
Большой астероид - маленькая скорость, летит в случайном направлении. При разрушении распадается на несколько средних астероидов, и вы получаете +20 очков.<br />
Средний астероид - средняя скорость, летит в случайном направлении. При разрушении распадается на несколько маленьких астероидов, и вы получаете +60 очков.<br />
Маленький астероид - высокая скорость, летит в случайном направлении, при его разрушении вы получаете +100 очков.<br />
Корабль камикадзе - быстро движется к вам. При уничтожении вы получаете +50 очков.<br />
Корабль стрелок - быстро движется к вам. При уничтожении вы получаете +200 очков.<br />

## **Как создать и скомпилировать этот проект в Visual Studio?**<br />
ЗАМЕТКА: у вас должна быть установлена Visual Studio 2022, которая поддерживает стандарт C++20. Гуглите, как её установить.<br />

1. Скачайте этот репозиторий как .zip файл и розархивируйте его.<br />
![2](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/97026464-e1ae-4787-820d-d5aeabf59556)

2. Создайте пустой C++ проект в Visual Studio.<br />
![3](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/ba48864e-86ff-421e-8f27-5be65d026eda)

3. Откройте папку проекта в проводнике и переместите все файлы из архива туда.<br />
![image](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/a061ec73-8441-4bed-ab4b-b5b9e8afce44)

4. Чтобы сделать все эти файлы видимыми в вашем проекте, нажтиме на кнопку "Show all files" в Solution Explorer.<br />
![4](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/21533c25-f96e-4e53-bbb8-40ffdc63f1c3)

5. Выберите все файлы в Solution Explorer, нажмите ПКМ и выберите "Include In Project" (некоторые файлы во внутрених папках могут не подключиться, поэтому вы можете подключить их индивидуально).<br />
![image](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/e99f90ad-0c66-4e97-ba13-0b715ba0a52a)

6. Нам нужно подключить библиотеку SFML к проекту и изменить C++ стандарт на C++20. Поэтому идите в настройки проекта.<br />
![5](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/bf9e841d-9119-49db-a0cf-107d75c39767)

7. Выберите "All Configurations" и "All Platforms".<br />
![image](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/32a7b835-c44a-4807-88ef-f1aff00f1456)

8. В "Configuration Properties" перейдите ко вкладке "General", найдите "C++ Language Standard" и выберите "ISO C++20 Standard (/std:c++20".<br />
![image](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/30d7c9f7-aefa-44aa-b352-f6d993872c4e)

9. Библиотека SFML состоит из 3 частей: .h/.cpp файлы (папка include), .lib файлы (папка lib) и .dll файлы. Давайте подключим сначала папку "include". Перейдите ко вкладке "C/C++", найдите пункт "Additional Include Directories", нажмите на стрелочку справа и нажмите "<Edit...>".<br />
![8](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/79cb8d11-aabb-40e5-897f-ddbf3fe087c1)

10. В появившемся окне дважды нажмите на пустую строку и напишите "$(ProjectDir)SFML\include", после чего нажмите кнопку "ОК" снизу окна.<br />
![9](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/4257e884-5b7f-41da-b223-804560326285)

11. Вам нужно сделать то же самое с .lib файлами: перейдите ко вкладке "Linker", найдите пункт "Additional Library Directories", нажмите на стрелочку справа и нажмите "<Edit...>.<br />
![10](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/3ada0b06-2495-444c-ba47-03de46a538f5)

12. Сделайте то же, что и в пункте №10, но теперь напишите "$(ProjectDir)SFML\lib".<br />
![image](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/a0488d5d-414c-4050-9a61-9f9ae3860f52)

13. Почти готово. Нам только нужно добавить .dll файлы в проект. Сохраните ваши изменения, нажав кнопку "Apply" снизу окна настроек проекта, измените конфигурацию на "Debug", перейдите ко вкладке "Linker" -> "Input", найдите пункт "Additional Dependencies", нажмите на стрелочку справа и нажмите "<Edit...>".<br />
![11](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/d6be1795-e5a9-49c4-b285-0bf18b07ed25)

14. В окне, которое появилось, напишите следующие строки:<br />
sfml-system-d.lib<br />
sfml-window-d.lib<br />
sfml-audio-d.lib<br />
sfml-graphics-d.lib<br />
sfml-network-d.lib<br />
и нажмите кнопку "Ok".<br />
![image](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/58e2669e-8805-4624-b2a5-aaf502f12297)

15. Нажмите "Apply", поменяйте конфигурацию на "Release" и сделайте то же самое, только напишите следующие строки:<br />
sfml-system.lib<br />
sfml-window.lib<br />
sfml-audio.lib<br />
sfml-graphics.lib<br />
sfml-network.lib<br />
и нажмите кнопку "Ok".<br />
![12](https://github.com/demianblogan/Game-Until_Last_Asteroid/assets/105989117/3f3f6dd1-6dae-46f0-8f26-6a9c873685c7)

16. Вот и всё! Нажмите "Apply", и теперь библиотека SFML подключена к вашему проекту.

17. Чтобы скомпилировать и запустить игру, нажмите "Ctrl + F5".
