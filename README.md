# Hospital

#include <iostream>
#include <math.h>
using namespace std;
int main()
{
    int days;
    float total1,total2,telephone,television ;
    char room,answer1,answer2;

    cout<<endl;
    cout<<"            ******************************************"<<endl;
    cout<<"            *******                            *******"<<endl;
    cout<<"            ***** Maple Valley Community Hospital ****"<<endl;
    cout<<"            *******                            *******"<<endl;
    cout<<"            ******           ( )_( )            ******"<<endl;
    cout<<"            *******          ( 'x' )            ******"<<endl;
    cout<<"            *******          C(O)(O)            ******"<<endl;
    cout<<"            ******************************************"<<endl;
    cout<<""<<endl;
    cout<<""<<endl;


    cout<<"Enter number of days spent in hospital\n";
    cin>>days;
    cout<<"Room provided. P for Private, S for Semiprivate Room or W for Ward\n";
    cin>>room;
    cout<<"Would you like to have a telephone in your room? Y or y for YES or N or n for NO"<<endl;
    cin>>answer1;
    cout<<"Would you like to have a TV in your room? Y or y for YES or N or n for NO\n"<<endl;
    cin>>answer2;
    
        if (answer1=='Y'||answer1=='y')
        telephone=1.75;
        else
        telephone= 0;
                total1=telephone*days;
        if (answer2=='Y'||answer2=='y')
        television= 3.50;
        else
        television= 0;
            total2=television*days;

        cout<<endl;
        cout<<endl;

    if (room=='p'||answer1=='P')
      {
        cout<<"Number of days in hospital   "<<days<<endl;
        cout<<"Type of Room:                "<<"Private"<<endl;
        cout<<"Telephone Charge:           $"<<total1<<endl;
        cout<<"Television Charge:          $"<<total2<<endl;
        cout<<"Total Due:                  $"<<days*125+total1+total2<<endl;
      }
    else if (room=='s'||answer1=='S')
        {
        cout<<"Number of days in hospital   "<<days<<endl;
        cout<<"Type of Room:                "<<"Semiprivate Room"<<endl;
        cout<<"Telephone Charge:           $"<<total1<<endl;
        cout<<"Television Charge:          $"<<total2<<endl;
        cout<<"Total Due:                  $"<<days*95+total1+total2<<endl;

        }
    else if (room=='w'||answer1=='W')
    {

        cout<<"Number of days in hospital   "<<days<<endl;
        cout<<"Type of Room:                "<<"Ward"<<endl;
        cout<<"Telephone Charge:           $"<<total1<<endl;
        cout<<"Television Charge:          $"<<total2<<endl;
        cout<<"Total Due:                  $"<<days*75+total1+total2<<endl;
    }
        return 0;
}

