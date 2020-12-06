# Register
//This program shows a list of students with their details
//The program uses classes and objects
#include <iostream>
#include <string>
using namespace std;

class students{
private:
//data member
string student_name;
string student_reg;
string student_course;
double student_age;
public:
//member function
void setData(string studname, string studreg, string studcourse,double studage)
{
    student_name=studname;
    student_reg=studreg;
    student_course=studcourse;
    student_age=studage;
}
void displayData()
{
    cout<<"students list"<<endl<<endl;
    cout<<"student name-"<<student_name<<endl;
    cout<<"student Reg No-"<<student_reg<<endl;
    cout<<"student course-"<<student_course<<endl;
    cout<<"student age-"<<student_age<<endl;
}
};

int main()//Introducing the variables for for the class (students)
{
    students student1;
    student1.setData("Karanja","E021-01-089/2021","Electrical Engineering",18);
    student1.displayData();
    students student2;
    student2.setData("James","B011-02-667/2021","BPSM",22);
    student2.displayData();
    return 0;
}
