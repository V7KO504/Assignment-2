#include <iostream>
#include <string>

using namespace std;

class Student {
private:
    string name;
    int age;
    float grade;

public:
    Student(string n, int a, float g) : name(n), age(a), grade(g) {}

    void display() {
        cout << "Name: " << name << ", Age: " << age << ", Grade: " << grade << endl;
    }

    void modifyGrade(float newGrade) {
        grade = newGrade;
    }

    void modifyAge(int newAge) {
        age = newAge;
    }
};

int main() {
    Student victor("Victor", 25, 75.5);
    victor.display();

    victor.modifyGrade(90.0);
    victor.modifyAge(21);
    
    victor.display();
    return 0;
}
