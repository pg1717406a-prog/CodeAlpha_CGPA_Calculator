#include <iostream>
#include <vector>
#include <iomanip>
using namespace std;

int main()
{
    int n;
    cout << "===== CGPA Calculator =====" << endl;

    cout << "Enter number of courses: ";
    cin >> n;

    vector<float> grade(n), credit(n);

    float totalGradePoints = 0;
    float totalCredits = 0;

    for(int i = 0; i < n; i++)
    {
        cout << "\nCourse " << i + 1 << endl;

        cout << "Enter Grade Point: ";
        cin >> grade[i];

        cout << "Enter Credit Hours: ";
        cin >> credit[i];

        totalGradePoints += grade[i] * credit[i];
        totalCredits += credit[i];
    }

    float cgpa = totalGradePoints / totalCredits;

    cout << "\n===== Course Details =====" << endl;

    for(int i = 0; i < n; i++)
    {
        cout << "Course " << i + 1
             << " | Grade Point: " << grade[i]
             << " | Credit Hours: " << credit[i]
             << endl;
    }

    cout << "\nTotal Credits: " << totalCredits << endl;
    cout << "Total Grade Points: " << totalGradePoints << endl;

    cout << fixed << setprecision(2);
    cout << "\nYour CGPA is: " << cgpa << endl;

    return 0;
}