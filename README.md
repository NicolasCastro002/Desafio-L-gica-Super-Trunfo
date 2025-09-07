# Desafio-L-gica-Super-Trunfo
#include <stdio.h>

int main() {
    // Atributos do jogador
    int ataqueJogador = 80;
    int defesaJogador = 70;
    int velocidadeJogador = 90;

    // Atributos da CPU
    int ataqueCPU = 75;
    int defesaCPU = 80;
    int velocidadeCPU = 90;

    // Contadores para atributos maiores
    int pontosJogador = 0;
    int pontosCPU = 0;

    // Comparando ataque
    if (ataqueJogador > ataqueCPU) {
        pontosJogador++;
    } else if (ataqueCPU > ataqueJogador) {
        pontosCPU++;
    }

    // Comparando defesa
    if (defesaJogador > defesaCPU) {
        pontosJogador++;
    } else if (defesaCPU > defesaJogador) {
        pontosCPU++;
    }

    // Comparando velocidade
    if (velocidadeJogador > velocidadeCPU) {
        pontosJogador++;
    } else if (velocidadeCPU > velocidadeJogador) {
        pontosCPU++;
    }

    // Decisão final
    if (pontosJogador >= 2) {
        printf("Jogador venceu a rodada!\n");
    } else if (pontosCPU >= 2) {
        printf("CPU venceu a rodada!\n");
    } else {
        printf("Empate!\n");
    }

    return 0;
}
