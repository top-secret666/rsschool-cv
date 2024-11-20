## Stukalova Dana Andreevna

**Contacts:**

* **Email:** chupacabra2.0666@gmail.com
* **Phone number:** +375292710932
* **Discord:** ufo
* **GitHub:** https://github.com/top-secret666

** About yourself:**

I am a 2nd year student of Vitebsk State Technical University, Faculty of Information Technology and Robotics, specialty “Information Technology". I am passionate about web application development and strive to develop in the field of front-end development. In my work, I value accuracy, efficiency, teamwork, and I believe that the ability to learn quickly and hard work are one of my main advantages.

**Skills:**

* **Programming languages:** C++, C#, JavaScript, Java, HTML, CSS
* **Development Tools:** Visual Studio, Visual Studio Code, CodeBlocks, Git, IntelliJ IDEA, GitHub 

**Sample code:**
* **The game "Rock Paper Scissors Lizard Spock"** C++
  
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

**Education:**

* **Vitebsk State Technical University**: Information Technology (2023 - present)
* **Udemy**: Complete C++20 Visual and Practical Course: Zero to Mastery
* **Udemy**: Unreal Engine 5 C++ Developer: Learn C++ & Make Video Games
* **Udemy**: Make an Arduino Robot

**English language:**

* **Level:** Average
* **Experience:** Active use in work and study.Practice communication skills with native speakers.

**Experience:**

* **Project: “CV”**:: “Development of a simple website in HTML, CSS and JavaScript".
* **Description:** This is my CV, which I developed using Markdown.
* **Link to the code:** https://github.com/top-secret666/rsschool-cv
  
* **Project: “MALAKA”**:: “Website development on ASP.NETCore".
* **Description:** This is my art goods store with its own catalog, shopping cart and registration, which I developed using the platform ASP.NET . The C# programming language.