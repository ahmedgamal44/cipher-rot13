# cipher-rot13
#include<bits/stdc++.h>

using namespace std;

int main()
{
    int q;
    cout<<" Cipher(1) & Decipher(2)? ";
    cin>>q;

    while ((q!=1)&&(q!=2))
    {
        cout<<"no more option"<<endl;
        cin>>q;
    }

    if (q==1)
    {
         string word;
        cout<<"enter massage: ";
        cin.ignore();
        getline(cin,word);
        for (int i = 0 ; i<word.length() ; i++)
        {

            int z,c;
            z=word[i];
            if((z>=97)  && (z<=109))
            {
                c= z + 13  ;
                cout<<  char(c);

            }
            if((z>109)  && (z<=122))
            {
                c= z - 13  ;
                cout<<  char(c);

            }
            if (z==32)
            {
                cout<<char(32);
            }

        }

    }
    if(q==2)
    {
        string word;
        cout<<"enter massage: ";
        cin.ignore();
        getline(cin,word);
        for (int i = 0 ; i<word.length() ; i++)
        {
            int z,c;
            z=word[i];
            if((z>=97)  && (z<=109))
            {
                c= z + 13  ;
                cout<<  char(c);

            }
            if((z>109)  && (z<=122))
            {
                c= z - 13  ;
                cout<<  char(c);

            }
            if (z==32)
            {
                cout<<char(32);
            }

        }
    }


    return 0;
}




