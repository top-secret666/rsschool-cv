# Dana Stukalova
## Front-End Developer

![Profile Photo](assets/img/profile-photo.jpg)

## 🎯 About Me

Passionate front-end developer and 2nd year student at Vitebsk State Technical University, Faculty of Information Technology and Robotics. I combine strong technical skills with creative problem-solving abilities. My focus is on delivering clean, efficient code while continuously learning new technologies.

## 📞 Contact Information

- 📧 Email: chupacabra2.0666@gmail.com
- 📱 Phone: +375292710932
- 💬 Discord: ufo
- 🔗 GitHub: [top-secret666](https://github.com/top-secret666)

## 💻 Technical Skills

### Programming Languages
- JavaScript
- C++
- C#
- Java
- HTML/CSS

### Development Tools
- Visual Studio
- Visual Studio Code
- CodeBlocks
- Git & GitHub
- IntelliJ IDEA

## 🎓 Education

### Vitebsk State Technical University
- **Program:** Information Technology
- **Period:** 2023 - Present

### Online Certifications
- Complete C++20 Visual and Practical Course (Udemy)
- Unreal Engine 5 C++ Developer (Udemy)
- Make an Arduino Robot (Udemy)

## 💼 Projects

### CV Website
- **Type:** Personal Project
- **Technologies:** HTML, CSS, JavaScript, Markdown
- **Repository:** [rsschool-cv](https://github.com/top-secret666/rsschool-cv)
- **Description:** Personal CV website showcasing my skills and experience

### MALAKA Art Store
- **Type:** E-commerce Platform
- **Technologies:** ASP.NET Core, C#
- **Features:** Product catalog, shopping cart, user authentication
- **Description:** Full-featured online store for art supplies

## 🌟 Featured Code Sample

The game "Rock Paper Scissors Lizard Spock:

```cpp
#include <iostream>
#include <Windows.h>
#include <string>
#include <ctime>

using namespace std;

string getSHELDONChoice() {
string choices[] = { "rock", "scissors", "paper", "lizard", "spock" };
    int randomIndex = rand() % 5;
    return choices[randomIndex];
}

string whoWinner(string youChoice, string sheldonChoice) {
    string winnerDict[5][2] = {
      {"scissors", "lizard"}, // Stone defeats Scissors and Lizard
      {"paper", "spock"}, // Scissors defeat Paper and Spock
      {"stone", "lizard"}, // Paper defeats Stone and Lizard
      {"spock", "paper"}, // The lizard defeats Spock and Paper
      {"rock", "scissors"}   // Spock defeats Rock and Scissors
    };
    if (youChoice == sheldonChoice) {
return "Draw!\n-LET'S DO IT AGAIN!!!!!!!!!";
}
    for (int i = 0; i < 2; ++i) {
        if (winnerDict[youChoice[0] - 'a'][i] == sheldonChoice) {
            return "You have won!\n-IT'S NOT FAIR, LET'S DO IT AGAIN, I'LL BEAT YOU ANYWAY!!!!!";
}
    }
return "Sheldon has won!\n-BUGAGASHENKI! HA HA";
}

void playRound(string youChoice) {
    string sheldonChoice = getSHELDONChoice();
    string winner = whoWinner(youChoice, sheldonChoice);
    cout << "You have chosen: " << youChoice << endl;
    cout << "Sheldon chose: " << sheldonChoice << endl;
    cout << winner << endl;
}

int main() {
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);
    srand(time(0));
    string youChoice;
    cout << "Enter your choice (rock, scissors, paper, lizard, spock): ";
cin >> youChoice;
    playRound(youChoice);
    return 0;
}
```