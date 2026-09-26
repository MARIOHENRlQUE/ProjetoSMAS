# Relatório Executivo — Sistema de Medição e Análise de Software (SMAS)

**Instituição:** UNIFAN  
**Disciplina/Contexto:** Relatório Executivo - Atividade Acadêmica  
**Professora Orientadora:** Soraia  
**Ano:** 2026  

## 👥 Autores
* João Pedro Pereira dos Santos e Santos
* Mario Henrique Pereira de Assis

## 📄 Sobre o Projeto
Este repositório contém o código-fonte em LaTeX do relatório executivo focado na **estabilidade e qualidade do módulo de pagamentos da RetailTech**. 

O documento propõe um Sistema de Medição e Análise de Software (SMAS) para tratar instabilidades no fluxo de checkout de um e-commerce de alto volume. A proposta engloba a utilização de atributos de qualidade da ISO/IEC 25010, estratégias de testes, gestão de fluxo com análise de valor agregado (EVM) e o alinhamento com o MPS.BR nível G.

## 📑 Estrutura do Documento
O relatório está dividido nos seguintes capítulos:
1. **Introdução:** Contextualização do problema na RetailTech e os objetivos do SMAS.
2. **Desenvolvimento:** 
   * Arquitetura e viabilidade (Cálculo do Custo da Não Qualidade - CNQ).
   * Gestão de defeitos e contenção.
   * Atributos de qualidade e rastreabilidade (ISO/IEC 25010).
   * Estratégia e métricas de testes.
   * Dashboard, fluxo e Análise de Valor Agregado (SPI, CPI).
   * Comunicação, saúde do time e código de ética.
   * Consolidação das práticas no modelo MPS.BR (Nível G).
3. **Análise Crítica:** Avaliação sobre a adoção da medição, riscos e mitigação de *gaming* com métricas.
4. **Conclusão:** Próximos passos e fechamento.

## 🛠️ Como compilar o projeto

Este documento foi escrito em **LaTeX** utilizando a classe `abntex2` para formatação nas normas da ABNT.

### Pré-requisitos
Para compilar o arquivo `.tex` e gerar o PDF, você precisará de:
* Uma distribuição LaTeX instalada (como [TeX Live](https://www.tug.org/texlive/) no Linux/Windows/Mac ou [MiKTeX](https://miktex.org/)).
* Pacote `abntex2` e dependências padrões do LaTeX (como `microtype`, `graphicx`, `booktabs`, `amsmath`, etc).

### Compilação via Terminal
Abra o terminal no diretório onde o arquivo `main.tex` está localizado e execute um dos comandos abaixo:

**Opção 1: Usando `latexmk` (Recomendado)**
```bash
latexmk -pdf main.tex
```

**Opção 2: Usando `pdflatex` manualmente**
Como o documento possui sumário (`\tableofcontents`), é necessário compilar duas vezes para que as referências de página fiquem corretas:
```bash
pdflatex main.tex
pdflatex main.tex
```

O arquivo gerado será o `main.pdf`.

## 📂 Arquivos Principais
* `main.tex`: Arquivo principal contendo todo o texto e estrutura do relatório.
* `main.log`: Log de compilação do LaTeX gerado durante a construção do documento.
* `main.pdf`: (Após compilação) O relatório final formatado para leitura.