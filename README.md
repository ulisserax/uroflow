# uroflow
Machine Learning project to audio extraction and to develop a product to predict a prostatic problem in men through the uro flow rate test

Audio Data handling using python
Representada por parâmetros como frequencia, tamanho de banda, decibel, etc. 
Um áudio de sinal pode ser expressado como uma função de amplitude e tempo.
Exemplo de formatos que podem ser lidos pelo computador: wav, mp3, WMA
Ferramentas que podem ser utilizadas em python: Librosa e PyAudio
Spectograma: maneira visual de representar a força do sinal presente em uma onda. Atraves dele podemos ver como os níveis de energia variam com o tempo e aonde tem mais ou menos energia.
Para analisar áudio, devemos extrair o que é relevante para o problema (Extração de recursos).
1.    Centróide espectral: indica em qual frequencia a energia de um spectrum está centrado (o “centro da massa” do som). Indicado para diferenciar entre ruídos, fala ou música. É a medida para evidenciar se o espectro contém uma predominância de altas ou baixas frequências.
2.    Spectral Rolloff: medida da forma do sinal. Representa a frequencia na qual altas frequencias declinam a zero
3.    Spectral bandwith: definido como o tamanho da banda de luz e tamanho inteiro em sua máxima metade. 
4.    Zero-Crossing Rate: jeito simples de medir a maciez do sinal para calcular a oscilação. Tem valores maiores para sons mais percursivos como metal e rock. Muito utilizado para discernir entre voz e música. Voz vocais e não-vocais possuem baixas taxas de ZCR, o que significa uma grande variação de ZCR. No caso de músicas, não há essa variação significativa da taxa de ZCR.
5.    MFCC: pequeno set de recursos que descreve a forma geral de um envelope espectral.
6.    Recurso Chroma: vetor de 12 elementos indicando quanta energia de cada nota está presente no sinal. Permite uma maneira robusta de descrever a medida de similaridade entre partes de músicas.
7.    STE (Short-Time-Energy): Sequência temporal quadrática do domínio de um dado (somatória de amostras de uma janela de processos). É a medida de energia de um sinal, muito utilizado para discernir entre música ou fala. Para falas, geralmente, STE possui uma grande variação comparada com uma música.
8.    RMS (Root-Mean-Square): Também é uma medida de energia em um sinal sonoro (uma expressão matemática mais complexa que STE - Raíz quadrada do STE/Quantidade de amostras). Mesma ideia para discernir fala de música e com variações também similar.
9.    HZCRR (High-Zero-Crossing-Rate-Ratio): É definido como a razão do número de cenas do gráfico cujo ZCR é acima de 1,5 em 1 segundo.
10.   LSTER (Low-Short-Time-Energy-Ratio): É definido como a razão do número de cenas do gráfico (regiões do gráfico) cujo STE esteja abaixo de 0,5 em 1 segundo.
11.   Spectrum Spread: Está intimamente relacionado com o centróide espectral. É a medida que sinaliza se o espectro de potência está concentrado em torno do centróide ou distribuído ao longo do espectro. No âmbito musical, rock possui uma maior potência espectral do que uma música calma com flautas.
12.   Delta Spectrum: Diferencia entre música ou sons ambiente.
@Ulissera
Ver todos os atributos possíveis para aplicar nas ondas sonoras das gravações para depois fazer a comparação entre as ondas saudáveis e doentes.
