#include <stdio.h>

// Constantes para o tamanho do tabuleiro
#define LINHAS 8
#define COLUNAS 8

int main() {
    printf("=== BATALHA NAVAL - NÍVEL NOVATO ===\n\n");
    
    // Declaração do tabuleiro (matriz 8x8)
    // 0 representa água, 1 representa parte de um navio
    int tabuleiro[LINHAS][COLUNAS] = {0};
    
    // 1. POSICIONAMENTO DO NAVIO HORIZONTAL
    printf("--- Posicionando Navio Horizontal ---\n");
    
    // Coordenadas do navio horizontal (linha 2, colunas 3 a 5)
    int navio_horizontal_linha = 2;
    int navio_horizontal_coluna_inicio = 3;
    int navio_horizontal_tamanho = 3;
    
    // Posicionando o navio horizontal no tabuleiro
    for(int coluna = navio_horizontal_coluna_inicio; 
        coluna < navio_horizontal_coluna_inicio + navio_horizontal_tamanho; 
        coluna++) {
        tabuleiro[navio_horizontal_linha][coluna] = 1;
        printf("Navio horizontal - Parte %d: (%d, %d)\n", 
               coluna - navio_horizontal_coluna_inicio + 1,
               navio_horizontal_linha, coluna);
    }
    printf("\n");
    
    // 2. POSICIONAMENTO DO NAVIO VERTICAL
    printf("--- Posicionando Navio Vertical ---\n");
    
    // Coordenadas do navio vertical (coluna 6, linhas 4 a 6)
    int navio_vertical_coluna = 6;
    int navio_vertical_linha_inicio = 4;
    int navio_vertical_tamanho = 3;
    
    // Posicionando o navio vertical no tabuleiro
    for(int linha = navio_vertical_linha_inicio; 
        linha < navio_vertical_linha_inicio + navio_vertical_tamanho; 
        linha++) {
        tabuleiro[linha][navio_vertical_coluna] = 1;
        printf("Navio vertical - Parte %d: (%d, %d)\n", 
               linha - navio_vertical_linha_inicio + 1,
               linha, navio_vertical_coluna);
    }
    printf("\n");
    
    // 3. EXIBIÇÃO DAS COORDENADAS COMPLETAS
    printf("=== COORDENADAS DOS NAVIOS ===\n\n");
    
    printf("NAVIO HORIZONTAL:\n");
    printf("Tamanho: %d casas\n", navio_horizontal_tamanho);
    printf("Posição: Linha %d, Colunas %d a %d\n", 
           navio_horizontal_linha,
           navio_horizontal_coluna_inicio,
           navio_horizontal_coluna_inicio + navio_horizontal_tamanho - 1);
    
    for(int coluna = navio_horizontal_coluna_inicio; 
        coluna < navio_horizontal_coluna_inicio + navio_horizontal_tamanho; 
        coluna++) {
        printf("- Coordenada (%d, %d)\n", navio_horizontal_linha, coluna);
    }
    printf("\n");
    
    printf("NAVIO VERTICAL:\n");
    printf("Tamanho: %d casas\n", navio_vertical_tamanho);
    printf("Posição: Coluna %d, Linhas %d a %d\n", 
           navio_vertical_coluna,
           navio_vertical_linha_inicio,
           navio_vertical_linha_inicio + navio_vertical_tamanho - 1);
    
    for(int linha = navio_vertical_linha_inicio; 
        linha < navio_vertical_linha_inicio + navio_vertical_tamanho; 
        linha++) {
        printf("- Coordenada (%d, %d)\n", linha, navio_vertical_coluna);
    }
    printf("\n");
    
    // 4. VISUALIZAÇÃO DO TABULEIRO (OPCIONAL)
    printf("=== VISUALIZAÇÃO DO TABULEIRO ===\n\n");
    printf("Legenda: . = Água, N = Navio\n\n");
    printf("  ");
    for(int coluna = 0; coluna < COLUNAS; coluna++) {
        printf("%d ", coluna);
    }
    printf("\n");
    
    for(int linha = 0; linha < LINHAS; linha++) {
        printf("%d ", linha);
        for(int coluna = 0; coluna < COLUNAS; coluna++) {
            if(tabuleiro[linha][coluna] == 1) {
                printf("N ");
            } else {
                printf(". ");
            }
        }
        printf("\n");
    }
    
    return 0;
}
