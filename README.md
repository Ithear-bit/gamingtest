#include <iostream>
#include <string>

using namespace std;

int main() {
    string text = "123123123123123123123123123123123123123123123123123123123123123123123123123123"; // Исходный текст

    while (text.find("12") != string::npos || text.find("333") != string::npos) {
        if (text.find("12") != string::npos) {
            text.replace(text.find("12"), 2, "3"); // Заменяем "12" на "3"
        } else {
            text.replace(text.find("333"), 3, "3"); // Заменяем "333" на "3"
        }
    }

    cout << "Результат: " << text << endl; // Выводим результат
    return 0;
}
.