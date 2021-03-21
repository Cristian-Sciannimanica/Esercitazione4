#include <stdio.h>
#include <string.h>

//Input: sequenza binaria
//Output: numero di 1 nella sequenza binaria
int quanti_uno(char *sequenza) {
    int N = 0;
    int L = (int)strlen(sequenza);

    int i;
    for(i=0;i<L;i++){
        if(sequenza[i]=='1'){
            N++;
        }
    }
    return N;
}

int main(int argc, char *argv[]) {
    // data una sequenza binaria (si assume corretta) come primo ed unico parametro sulla linea di comando
    // calcolare il bit di parità pari e dispari
    // stampare come output le seguenti stringhe
    //
    // Calcolo bit parità per la sequenza <sequenza>:
    // bit parità pari = <1|0>
    // bit parità dispari = <1|0>

    // inserisci qui il tuo codice
    printf("%d\n", quanti_uno(argv[1]));
    return 0;
}
