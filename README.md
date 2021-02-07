#include <iostream>

using namespace std;
class student
{
    protected:
        int rollnumber;
    public:
        void get_number(int);
        void put_number(void);
    
};
void student :: get_number(int a)
{
    rollnumber=a;
}
void student :: put_number()
{
    cout<<"RollNumber\n"<<rollnumber<<"\n";
}
class test : public student
{
    protected:
        int Math;
        int Science;
        int ELA;
        int History;
    public:
        void get_score(float,float,float,float);
        void put_score(void);
};
void test :: get_score(float x,float y, float z, float b)
{
    Math = x;
    Science = y;
    ELA = z;
    History = b;
}
void test :: put_score()
{
    cout<<"Score in Math:\n"<<Math<<"\n";
    cout<<"Score in Science:\n"<<Science<<"\n";
    cout<<"Score in Ela:\n"<<ELA<<"\n";
    cout<<"Score in History:\n"<<History<<"\n";
}
class result : public test
{
    public:
        void display(void);
};
void result :: display(void)
{
    put_number();
    put_score();
};
int main()
{
    int i;
    result student1;
    student1.get_number(22);
    student1.display();
    cout<<"Enter the score you got in Math :";
    float mark, sum = 0, avg;
    for(i=0;i<1;i++)
    {
        cin>>mark;
        sum = sum+mark;
    }
    avg = sum/1;
    cout<<"\nGrade in math = ";
    if(avg>=95 && avg<=100)
        cout<<"A+";
    else if(avg>=90 && avg<=95)
        cout<<"A";
    else if(avg>=85 && avg<=90)
       cout<<"B+";
    else if(avg>=80 && avg<=85)
        cout<<"B";
    else if(avg>=75 && avg<=80)
        cout<<"C+";
   else if(avg>=70 && avg<=75)
        cout<<"C";
    else if(avg>=65 && avg<=70)
        cout<<"D+";
    else if(avg>=60 && avg<=65)
        cout<<"D";
    else if(avg>=0 && avg<=60)
        cout<<"F";
    else
       cout<<"Invalid!";
    cout<<endl;
    cout<<"\nEnter the score you got in Science: ";
    float marks1,sum1=0, avg1;
    for(i=0;i<1;i++)
    {
        cin>>marks1;
        sum1 = sum1+marks1;
    }
    avg1 = sum1/1;
    cout<<"\nGrade in Science = ";
    if(avg>=95 && avg<=100)
        cout<<"A+";
    else if(avg>=90 && avg<=95)
        cout<<"A";
    else if(avg>=85 && avg<=90)
       cout<<"B+";
    else if(avg>=80 && avg<=85)
        cout<<"B";
    else if(avg>=75 && avg<=80)
        cout<<"C+";
   else if(avg>=70 && avg<=75)
        cout<<"C";
    else if(avg>=65 && avg<=70)
        cout<<"D+";
    else if(avg>=60 && avg<=65)
        cout<<"D";
    else if(avg>=0 && avg<=60)
        cout<<"F";
    else
       cout<<"Invalid!";
    cout<<endl;
    cout<<"\nEnter the score you got in Ela:\n";
    float marks2, sum2=0, avg2;
    for(i=0;i<1;i++)
    {
        cin>>marks2;
        sum2 = sum2+marks2;
    }
    avg = sum2/1;
    cout<<"\nGrade in Reading = ";
    if(avg>=95 && avg<=100)
        cout<<"A+";
    else if(avg>=90 && avg<=95)
        cout<<"A";
    else if(avg>=85 && avg<=90)
       cout<<"B+";
    else if(avg>=80 && avg<=85)
        cout<<"B";
    else if(avg>=75 && avg<=80)
        cout<<"C+";
   else if(avg>=70 && avg<=75)
        cout<<"C";
    else if(avg>=65 && avg<=70)
        cout<<"D+";
    else if(avg>=60 && avg<=65)
        cout<<"D";
    else if(avg>=0 && avg<=60)
        cout<<"F";
    else
       cout<<"Invalid!";
    cout<<endl;
    cout<<"\nEnter the score you got in History:\n";
    float marks3, sum3, avg3;
    for(i=0;i<1;i++)
    {
        cin>>marks3;
        sum3 = sum3+marks3;
    }
    avg = sum3/1;
    cout<<"\nGrade in History = ";
    if(avg>=95 && avg<=100)
        cout<<"A+";
    else if(avg>=90 && avg<=95)
        cout<<"A";
    else if(avg>=85 && avg<=90)
       cout<<"B+";
    else if(avg>=80 && avg<=85)
        cout<<"B";
    else if(avg>=75 && avg<=80)
        cout<<"C+";
   else if(avg>=70 && avg<=75)
        cout<<"C";
    else if(avg>=65 && avg<=70)
        cout<<"D+";
    else if(avg>=60 && avg<=65)
        cout<<"D";
    else if(avg>=0 && avg<=60)
        cout<<"F";
    else
       cout<<"Invalid!";
    cout<<endl;
    return 0;
}
