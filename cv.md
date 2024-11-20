## Стукалова Дана Андреевна

**Контакты:**

* **Электронная почта:** chupacabra2.0666@gmail.com
* **Телефон:** +375292710932
* **Discord:** ufo
* **GitHub:** https://github.com/top-secret666

**О себе:**

Я - студентка 2 курса Витебского государственного технического университета, факультета информационных технологий и робототехники, специальности “Информационные технологии”. Я увлечена разработкой веб-приложений и стремлюсь развиваться в сфере front-end разработки. В своей работе я ценю аккуратность, эффективность, командную работу, и считаю, что способность быстро учиться и трудолюбие - одно из моих главных преимуществ.

**Навыки:**

* **Языки программирования:** C++, C#, JavaScript, Java, HTML, CSS
* **Инструменты разработки:** Visual Studio, Visual Studio Code, CodeBlocks, Git, IntelliJ IDEA, GitHub 

**Пример кода:**
* **Игра "Камень Ножницы Бумага Ящерица Спок"** C++
  
```cpp
#include <iostream>
#include <Windows.h>
#include <string>
#include <ctime>

using namespace std;

string getSHELDONChoice() {
    string choices[] = { "камень", "ножницы", "бумага", "ящерица", "спок" };
    int randomIndex = rand() % 5;
    return choices[randomIndex];
}

string whoWinner(string youChoice, string sheldonChoice) {
    string winnerDict[5][2] = {
      {"ножницы", "ящерица"}, // Камень побеждает Ножницы и Ящерицу
      {"бумага", "спок"},     // Ножницы побеждают Бумагу и Спока
      {"камень", "ящерица"},  // Бумага побеждает Камень и Ящерицу
      {"спок", "бумага"},     // Ящерица побеждает Спока и Бумагу
      {"камень", "ножницы"}   // Спок побеждает Камень и Ножницы
    };
    if (youChoice == sheldonChoice) {
        return "Ничья!\n-ДАВАЙ ЕЩЕ РАЗ!!!!!!!!!";
    }
    for (int i = 0; i < 2; ++i) {
        if (winnerDict[youChoice[0] - 'а'][i] == sheldonChoice) {
            return "Вы победили!\n-ТАК НЕЧЕСТНО ДАВАЙ ЕЩЕ РАЗ Я ВСЕ РАВНО ТЕБЯ ПОБЕДЮ!!!!!";
        }
    }
    return "Шелдон победил!\n-БУГАГАШЕНЬКИ! ХА-ХА";
}

void playRound(string youChoice) {
    string sheldonChoice = getSHELDONChoice();
    string winner = whoWinner(youChoice, sheldonChoice);
    cout << "Вы выбрали: " << youChoice << endl;
    cout << "Шелдон выбрал: " << sheldonChoice << endl;
    cout << winner << endl;
}

int main() {
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);
    srand(time(0));
    string youChoice;
    cout << "Введите свой выбор (камень, ножницы, бумага, ящерица, спок): ";
    cin >> youChoice;
    playRound(youChoice);
    return 0;
}
```

**Образование:**

* **Витебский государственный технический университет**: Информационные технологии (2023 - настоящее время)
* **Udemy**: Complete C++20 Visual and Practical Course: Zero to Mastery
* **Udemy**: Unreal Engine 5 C++ Developer: Learn C++ & Make Video Games
* **Udemy**: Make an Arduino Robot

**Английский язык:**

* **Уровень:** Средний
* **Опыт:** Активное использование в работе и учебе.Практика навыков общения с носителями языка.

**Опыт:**

* **Проект: “CV”**:: “Разработка простого веб-сайта на HTML, CSS и JavaScript”.
* **Описание:** Это моё CV, которое я разработала, используя Markdown.
* **Ссылка на код:** https://github.com/top-secret666/rsschool-cv
  
* **Проект: “МАЛЯКА”**:: “Разработка веб-сайта на ASP.NETCore”.
* **Описание:** Это мой магазин художественных товаров со своим каталогом, корзиной и регистрацией, которое я разработала, используя платформу ASP.NET. Язык программирования C#.

