# bci-ssvep
# Atividade Prática – Análise de Eletroencefalogramas (BCI-SSVEP)

Este repositório contém minha atividade prática da disciplina *IA006 – Introdução a Interfaces Cérebro-Computador*, cursada como aluna especial na Unicamp (1º semestre de 2025). A atividade foi desenvolvida com apoio de ferramentas de IA e bibliotecas científicas em Python.

---

## Objetivos

- Explorar um dataset público de EEGs com múltiplos usuários, eletrodos e estímulos visuais  
- Analisar os sinais nos domínios do tempo e da frequência  
- Investigar padrões de evocação cerebral relacionados ao paradigma SSVEP

## Conteúdo

- `relatorio.pdf`: relatório técnico com análise dos resultados
- `questoes.md`: questões teóricas da atividade
- `notebook/`: notebook original com código base em Python

## Cenário abordado: BCI-SSVEP

O paradigma SSVEP (steady-state visually evoked potentials) baseia-se na resposta cerebral sincronizada a estímulos visuais periódicos. Quando o usuário foca em um estímulo piscante com frequência específica, ocorre aumento de energia cerebral nessa frequência e suas harmônicas, especialmente na região occipital do córtex.

## Base de dados

Utiliza o [Benchmark Dataset da Universidade de Tsinghua](https://bci.med.tsinghua.edu.cn/download.html), com arquivos `.mat` contendo sinais de 64 eletrodos posicionados segundo o padrão internacional 10-10.

## Ferramentas utilizadas

- Python  
- Bibliotecas: `scipy.io`, `scipy.signal`, `matplotlib`, `numpy`  
- Visualizações: sinal no tempo, FFT, PSD via Welch, espectrograma  
- Pré-processamento: filtro passa-altas (>3 Hz)

## Referências

- Wang et al., 2017 – *A Benchmark Dataset for SSVEP-Based Brain–Computer Interfaces*, IEEE TNSRE  
- Wolpaw et al., 2002 – *Brain-computer interfaces for communication and control*, Clinical Neurophysiology
