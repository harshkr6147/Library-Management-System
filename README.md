#include <iostream>

using namespace std;

class library{
    int reg_no,book_no;
    string name,branch;
public:
    void set_details(void){
        cout<<"Eneter your name:"<<"\n";
        cin>>name;

        cout<<"Enter your registration no.:"<<"\n";
        cin>>reg_no;

        cout<<"Enter your branch"<<"\n";
        cin>>branch;
        cout<<"\n";
        }

     void display_details(void){
        cout<<"Name :"<<name<<"\n";
        cout<<"Registration No. :"<<reg_no<<"\n";
        cout<<"Branch :"<<branch<<"\n";
        cout<<"\n";
     }

     void ask_book(void){
        cout<<"Enter your Book no. :"<<"\n";
        cin>>book_no;
        cout<<"Book with "<<book_no<<" has been issued to "<<name<<" for 14 days"<<"\n";
        cout<<"After that a fine of Rs1/day will be charged";
     }
};
int main()
{
    library std1;
    std1.set_details();
    std1.display_details();
    std1.ask_book();
    cout << "" << endl;
    return 0;
}

