# Respostas do teste de nível
// Luiz Eduardo de Almeida Rodrigues

// Questão 01
#include <stdio.h>

void inverterVetor(int vet[], int n) {
    int temp;
    for (int i = 0; i < n / 2; i++) {
        temp = vet[i];
        vet[i] = vet[n - 1 - i];
        vet[n - 1 - i] = temp;
    }
}

int main() {
    int tamanho = 5;
    int meuVetor[] = {1, 2, 3, 4, 5};  

    printf("Vetor original: ");
    for (int i = 0; i < tamanho; i++) {
        printf("%d ", meuVetor[i]);
    }

    inverterVetor(meuVetor, tamanho);

    printf("\nVetor invertido: ");
    for (int i = 0; i < tamanho; i++) {
        printf("%d ", meuVetor[i]);
    }

    return 0;
}

// Questão 3
// Falta ponto e vírgula na declaração das variáveis. Falta declarar a variável "i" e seu tipo no "for". "return" deveria ser "return 0;"

// Questão 4
#include <stdio.h>

int somaNumerosInteiros(int a, int b) {
    int soma = 0;

    if (a > b) {
        int temp = a;
        a = b;
        b = temp;
    }

    for (int i = a; i <= b; i++) {
        soma += i;
    }

    return soma;
}

int main() {
    int num1, num2;

    printf("Digite o primeiro numero positivo: ");
    scanf("%d", &num1);

    printf("Digite o segundo numero positivo: ");
    scanf("%d", &num2);

    int resultado = somaNumerosInteiros(num1, num2);
    printf("A soma dos numeros inteiros entre %d e %d é: %d\n", num1, num2, resultado);

    return 0;
}

// Questão 5
// 2
// 200
// Fim do laco!
