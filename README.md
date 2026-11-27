# -#include <iostream>
#include <fstream>
#include <string>

using namespace std;

int main() {
    string fullName, id, grade;

    cout << "Enter Full Name: ";
    getline(cin, fullName);

    cout << "Enter ID: ";
    getline(cin, id);

    cout << "Enter Grade: ";
    getline(cin, grade);

    ofstream file("Student.txt");
    file << "Full Name: " << fullName << endl;
    file << "ID: " << id << endl;
    file << "Grade: " << grade << endl;
    file.close();

    cout << "Done!" << endl;
    return 0;
}