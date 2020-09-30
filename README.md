# Ordem_Crescente_Descrescente
C++

#include <iostream>

using namespace std;

int main()
{
   int v[10];
   int aux;
    
    cout<<"Vetor v[i]"<<endl;
    srand(time(NULL));
    for(int i=0;i<10;i++){
        v[i]=rand()%11;
        cout<<"["<<v[i]<<"]"<<" ";
    }
        cout<<endl;
        cout<<endl;
        cout<<"ORDEM CRESCENTE"<<endl;
        for(int i=0;i<10;i++){
            for(int j=i+1;j<10;j++){
                if(v[i]>v[j]){
                    aux = v[i];
                    v[i] = v[j];
                    v[j] = aux;
                }
            }
            cout<<"----->"<<v[i];
        }
            cout<<endl;
            cout<<endl;
            cout<<"ORDEM DECRESCENTE"<<endl;
            for(int i=0;i<10;i++){
                for(int j=i+1;j<10;j++){
                    if(v[i]<v[j]){
                        aux = v[i];
                        v[i] = v[j];
                        v[j] = aux;
                    }
                }
                cout<<"----->"<<v[i];
            }
    return 0;
}
