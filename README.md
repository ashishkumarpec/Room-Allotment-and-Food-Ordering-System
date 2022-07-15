# Room-Allotment-and-Food-Ordering-System

#include <iostream>

using namespace std;

int main()
{
    int quant;
    int choice;
    //Quantity
    int Qrooms=0, Qpasta=0, Qburger=0, Qnoodles=0,Qshake=0, Qchicken=0;
    //food items sold
    int Srooms=0, Spasta=0, Sburger=0, Snoodles=0, Sshake=0, Schicken=0;
    //Total price of items
    int Total_rooms=0, Total_pasta=0, Total_burger=0,Total_noodles=0, Total_shake=0, Total_chicken=0;

    cout<<"\n\t Quantity of items we have";
    cout<<"\n Rooms available ";
    cin>>Qrooms;
    cout<<"\n Quantity of pasta: ";
    cin>>Qpasta;
    cout<<"\n Quantity of burger: ";
    cin>>Qburger;
    cout<<"\n Quantity of noodles: ";
    cin>>Qnoodles;
    cout<<"\n Quantity of shake: ";
    cin>>Qshake;
    cout<<"\n Quantity of Chicken-rolls: ";
    cin>>Qchicken;

    m:
    cout<<"\n\t\t\t Please select from the menu options ";
    cout<<"\n\n 1) Rooms ";
    cout<<"\n 2) Pasta ";
    cout<<"\n 3) Burgers ";
    cout<<"\n 4) Noodles ";
    cout<<"\n 5) Shake ";
    cout<<"\n 6) Chicken-rolls ";
    cout<<"\n 7) Information regarding sales and Collection ";
    cout<<"\n 8) Exit ";

    cout<<"\n\n Please Enter your choice! ";
    cin>>choice;

    switch(choice){
    case 1:
        cout<<"\n\n Enter the number of rooms you want: ";
        cin>>quant;
        if(Qrooms-Srooms >=quant){
            Srooms=Srooms+quant;
            Total_rooms=Total_rooms+quant*1500;
            cout<<"\n\n\t\t"<<quant<<" room/rooms have been alloted to you!";
        }
        else{
            cout<<"\n\t Only"<<Qrooms-Srooms<<" Rooms remaining in hotel! ";
            break;
        }

            case 2:
        cout<<"\n\n Enter Pasta Quantity :" ;
        cin>>quant;
        if(Qpasta-Spasta >=quant){
            Spasta=Spasta+quant;
            Total_pasta=Total_pasta+quant*200;
            cout<<"\n\n\t\t"<<quant<<" Pasta is in order!";
        }
        else{
            cout<<"\n\t Only"<<Qpasta-Spasta<<" Pasta remaining in hotel! ";
            break;
        }
            case 3:
        cout<<"\n\n Enter the number of burger you want: ";
        cin>>quant;
        if(Qburger-Sburger >=quant){
            Sburger=Sburger+quant;
            Total_burger=Total_burger+quant*100;
            cout<<"\n\n\t\t"<<quant<<" Burger is in the order!";
        }
        else{
            cout<<"\n\t Only"<<Qburger-Sburger<<" Burger remaining in hotel! ";
            break;
        }
            case 4:
        cout<<"\n\n Enter the noodle quantity you want: ";
        cin>>quant;
        if(Qnoodles-Snoodles >=quant){
            Snoodles=Snoodles+quant;
            Total_noodles=Total_noodles+quant*140;
            cout<<"\n\n\t\t"<<quant<<" Noodle is in the order!";
        }
        else{
            cout<<"\n\t Only"<<Qnoodles-Snoodles<<" noodles remaining in hotel! ";
            break;
        }
        case 5:
        cout<<"\n\n Enter the shake quantity you want: ";
        cin>>quant;
        if(Qshake-Sshake>=quant){
            Sshake=Sshake+quant;
            Total_shake=Total_shake+quant*100;
            cout<<"\n\n\t\t"<<quant<<" shakes is in the order!";
        }
        else{
            cout<<"\n\t Only"<<Qshake-Sshake<<" shakes remaining in hotel! ";
            break;
        }
        case 6:
        cout<<"\n\n Enter the Chicken-roll quantity you want: ";
        cin>>quant;
        if(Qchicken-Schicken>=quant){
            Schicken=Schicken+quant;
            Total_chicken=Total_chicken+quant*100;
            cout<<"\n\n\t\t"<<quant<<" chicken-roll is in the order!";
        }
        else{
            cout<<"\n\t Only"<<Qchicken-Schicken<<" chicken-roll remaining in hotel! ";
            break;
        }
        case 7:
            cout<<"\n\t\tDetails of sales and collections ";
            cout<<"\n\n Number of rooms we had: "<<Qrooms;
            cout<<"\n\n Number of rooms we gave in booking "<<Srooms;
            cout<<"\n\n Remaining rooms :"<<Qrooms-Srooms;
            cout<<"\n\n Total rooms collection for the day : "<<Total_rooms;

            cout<<"\n\t\tDetails of sales and collections ";
            cout<<"\n\n Number of pastas we had: "<<Qpasta;
            cout<<"\n\n Number of pastas we gave in booking "<<Spasta;
            cout<<"\n\n Remaining pastas :"<<Qpasta-Spasta;
            cout<<"\n\n Total pastas collection for the day : "<<Total_pasta;

            cout<<"\n\t\tDetails of sales and collections ";
            cout<<"\n\n Number of burgers we had: "<<Qburger;
            cout<<"\n\n Number of burgers we gave in booking "<<Sburger;
            cout<<"\n\n Remaining burgers :"<<Qburger-Sburger;
            cout<<"\n\n Total burgers collection for the day : "<<Total_burger;

            cout<<"\n\t\tDetails of sales and collections ";
            cout<<"\n\n Number of noodles we had: "<<Qnoodles;
            cout<<"\n\n Number of noodles we gave in booking "<<Snoodles;
            cout<<"\n\n Remaining noodles :"<<Qnoodles-Snoodles;
            cout<<"\n\n Total noodles collection for the day : "<<Total_noodles;

            cout<<"\n\t\tDetails of sales and collections ";
            cout<<"\n\n Number of shakes we had: "<<Qshake;
            cout<<"\n\n Number of shakes we gave in booking "<<Sshake;
            cout<<"\n\n Remaining shakes :"<<Qshake-Sshake;
            cout<<"\n\n Total shakes collection for the day : "<<Total_shake;

            cout<<"\n\t\tDetails of sales and collections ";
            cout<<"\n\n Number of chicken-rolls we had: "<<Qchicken;
            cout<<"\n\n Number of chicken-rolls we gave in booking "<<Schicken;
            cout<<"\n\n Remaining chicken-rolls :"<<Qchicken-Schicken;
            cout<<"\n\n Total chicken-rolls collection for the day : "<<Total_chicken;

        case 8:
            exit(0);

        default:
            cout<<"\n Please select the numbers mentioned above! ";




    }
    //jump statement
    goto m;
}
