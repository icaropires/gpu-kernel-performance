# Aprendizagem de Máquina

## 2ª Rodada de Problemas - Grupo A

### Dataset

O Dataset do problema mede o tempo de execução de um produto matricial (A * B = C), no qual todas as matrizes possuem o tamanho 2048x2048. em um kernel GPU SGEMM parametrizável com 241600 combinações possíveis. Para cada combinação foram executados 4 testes, com a medição do tempo em milissegundos.

SGEMM é um método de multiplicação de matrizes gerais de precisão única que utiliza a algebra linear para o seu cálculo.

O dataset do problema pode ser encontrado [aqui](https://archive.ics.uci.edu/ml/datasets/SGEMM+GPU+kernel+performance#)

#### Conjunto de Dados

1. **MWG**
    * Colunas 1
    * **Descrição:** Dimensão da linha da submatriz 2D A.
    * **Domínio:** {16, 32, 64, 128} (Inteiro)
1. **NWG**
    * Colunas 2
    * **Descrição:** Dimensão da coluna da submatriz 2D B.
    * **Domínio:** {16, 32, 64, 128} (Inteiro)
1. **KWG**
    * Coluna 3
    * **Descrição:** Dimensão da linha da submatriz 2D B e coluna da submatriz 2D A.
    * **Domínio:** {16, 32} (Inteiro)
1. **MDIMC e NDIMC**
    * Colunas 4 a 5
    * **Descrição:** quantidades de _thrads_ utilizadas nas submatrizes M e N.
    * **Domínio:** {8, 16, 32} (Inteiro)
1. **MDIMA e NDIMB**
    * Colunas 6 a 7
    * **Descrição:** forma da memória local.
    * **Domínio:** {8, 16, 32} (Inteiro)
1. **KWI**
    * Coluna 8
    * **Descrição:** uma fatoração da matriz K.
    * **Domínio:** {2, 8} (Inteiro)
1. **VWM e VWN**
    * Colunas 9 a 10
    * **Descrição:** larguras do vetor por matriz para carregamento e armazenamento.
    * **Domínio:** {1, 2, 4, 8} (Inteiro)
1. **STRM e STRN**
    * Colunas 11 a 12
    * **Descrição:** _stride_ habilitado para acesso da memória fora do chip em uma única _thread_.
    * **Domínio:** {0, 1} (Categórico)
1. **SA e SB**
    * Colunas 13 a 14
    * **Descrição:** cache manual por matriz do bloco de grupo de trabalho.
    * **Domínio:** {0, 1} (Categórico)
