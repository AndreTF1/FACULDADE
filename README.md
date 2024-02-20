#include <stdio.h>

void desenharRetangulo(int numeroLinhas, int numeroColuna) {
    for (int i = 0; i < numeroLinhas; i++) {
        for (int j = 0; j < numeroColuna; j++) {
            printf("* ");  // Use qualquer caractere desejado para desenhar o retângulo
        }
        printf("\n");  // Muda para a próxima linha após desenhar uma linha completa
    }
}

int main() {
    int linha, coluna;

    printf("Digite um numero para o tamanho do retangulo: ");
    scanf("%d", &linha);
    printf("Digite um numero para o tamanho do retangulo: ");
    scanf("%d", &coluna);

    if (linha && coluna <= 0) {
        printf("Por favor, digite um numero maior que zero.\n");
    } else {
        desenharRetangulo(linha, coluna);
    }

return 0;
}
