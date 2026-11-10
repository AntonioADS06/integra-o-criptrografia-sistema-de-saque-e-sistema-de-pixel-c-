#Sistema de integração
# Sistema Integrado de Criptografia, Saque e Processamento de Pixels

## 1. Apresentação do Projeto

Este projeto consiste no desenvolvimento de um sistema integrado utilizando a linguagem de programação C, reunindo diferentes funcionalidades em uma única aplicação.

O sistema foi desenvolvido com o objetivo de aplicar conceitos fundamentais de programação, incluindo manipulação de arquivos, estruturas condicionais, funções, vetores, matrizes, algoritmos matemáticos e processamento de dados.

A aplicação é organizada em três módulos principais: criptografia e autenticação de usuários, sistema de saque bancário e processamento de imagens por pixels.

## 1.1 Objetivo Geral

Desenvolver uma aplicação integrada capaz de executar diferentes operações computacionais, aplicando conceitos de lógica de programação e linguagem C na resolução de problemas práticos.

## 1.2 Objetivos Específicos

- Implementar um mecanismo de criptografia utilizando a Cifra de César e sequências matemáticas.
- Desenvolver um sistema de cadastro e autenticação de usuários.
- Simular operações bancárias com validação de saques e controle de saldo.
- Aplicar conceitos de processamento de imagens por meio de matrizes de pixels.
- Utilizar arquivos para armazenamento de informações e resultados.
- Desenvolver funcionalidades independentes integradas em um menu principal.

## 2. Estrutura e Funcionalidades do Sistema

O programa possui três módulos funcionais, acessados por meio de um menu principal.

### 2.1 Módulo 1 — Criptografia e Autenticação

Este módulo implementa mecanismos de transformação de palavras utilizando a Cifra de César e diferentes sequências matemáticas.

**Funcionalidades implementadas:**

- Criptografia utilizando deslocamento de letras (SHIFT).
- Aplicação da sequência de Progressão Aritmética (PA).
- Aplicação da sequência de Progressão Geométrica (PG).
- Aplicação da sequência de Fibonacci.
- Aplicação da sequência de números primos.
- Comparação dos resultados obtidos pelas diferentes sequências.
- Cadastro e autenticação de usuários por senha.
- Armazenamento dos resultados em arquivos.

A aplicação permite escolher uma sequência específica ou comparar todas as quatro sequências disponíveis.

### 2.2 Módulo 2 — Sistema de Saque Bancário

O segundo módulo simula um sistema de saque bancário, utilizando validações para garantir que as operações respeitem as condições estabelecidas.

**Regras operacionais:**

- Saldo inicial definido em R$ 1.000,00.
- Autenticação do usuário antes da operação.
- Validação para impedir saques com valores iguais ou inferiores a zero.
- Verificação de valores múltiplos de cinco.
- Verificação de saldo disponível.
- Distribuição das notas utilizando os valores de R$ 100, R$ 50, R$ 20, R$ 10 e R$ 5.
- Atualização do saldo após a realização do saque.

O módulo utiliza estruturas condicionais e estruturas de repetição para validar as operações e calcular a quantidade de notas necessárias.

### 2.3 Módulo 3 — Processamento de Imagens por Pixels

O terceiro módulo trabalha com uma matriz de 16 × 16 posições, representando uma imagem em escala de cinza.

Cada posição da matriz armazena um valor correspondente à intensidade de um pixel, permitindo realizar análises matemáticas e identificação de objetos.

**Funcionalidades implementadas:**

- Leitura e processamento de uma matriz de pixels.
- Cálculo da soma e média das intensidades.
- Construção de histograma com oito faixas de intensidade.
- Segmentação da imagem utilizando limiar de 128.
- Geração de máscara binária para identificação do objeto.
- Cálculo da área ocupada pelo objeto.
- Identificação da caixa delimitadora.
- Cálculo de altura e largura.
- Determinação do centroide.
- Cálculo da taxa de ocupação.

O processamento permite identificar características geométricas do objeto presente na imagem, utilizando operações sobre matrizes e cálculos matemáticos.

## 3. Tecnologias e Recursos Utilizados

O desenvolvimento foi realizado utilizando os seguintes recursos:

| Tecnologia | Aplicação |
|---|---|
| Linguagem C | Desenvolvimento da aplicação |
| GCC | Compilação do programa |
| Visual Studio Code | Ambiente de desenvolvimento |
| Git | Controle de versão |
| GitHub | Hospedagem e documentação do projeto |

### 3.1 Bibliotecas utilizadas

- `stdio.h` — entrada e saída de dados.
- `stdlib.h` — funções auxiliares e conversão numérica.
- `string.h` — manipulação de strings.
- `ctype.h` — validação e manipulação de caracteres.
- `errno.h` — tratamento de erros de conversão.
- `limits.h` — limites dos tipos inteiros.

## 4. Estruturas e Conceitos de Programação

Durante o desenvolvimento foram aplicados diferentes conceitos fundamentais da linguagem C:

- **Variáveis:** armazenamento de valores e informações.
- **Funções:** organização e divisão das responsabilidades do programa.
- **Vetores:** armazenamento de sequências matemáticas e dados.
- **Matrizes:** representação e processamento da imagem.
- **Estruturas condicionais:** validação de entradas e decisões.
- **Laços de repetição:** execução de operações sequenciais.
- **Enum:** identificação dos diferentes tipos de sequências matemáticas.
- **Manipulação de arquivos:** leitura e gravação de informações.
- **Algoritmos matemáticos:** cálculos de média, área, centroide e sequências numéricas.

## 5. Organização e Funcionamento

O sistema inicia com o processo de cadastro da senha, caso ainda não exista um arquivo de credenciais.

Após essa etapa, o usuário tem acesso ao menu principal, que permite selecionar uma das funcionalidades disponíveis.

**Fluxo principal da aplicação:**

1. Inicialização do programa.
2. Cadastro ou verificação da senha.
3. Exibição do menu principal.
4. Seleção do módulo desejado.
5. Execução das operações correspondentes.
6. Retorno ao menu principal.
7. Encerramento do sistema.

## 6. Arquivos e Armazenamento

O projeto utiliza arquivos externos para manter informações e resultados das operações.

| Arquivo | Finalidade |
|---|---|
| `senha.dat` | Armazenamento da senha codificada |
| `resultado_criptografia.txt` | Registro dos resultados da criptografia |
| `log_criptografia.txt` | Histórico das operações de criptografia |

Os arquivos são utilizados para demonstrar a persistência de informações, permitindo armazenar dados além da execução atual do programa.

## 7. Compilação e Execução

Para executar o projeto, é necessário possuir um compilador GCC instalado e configurado.

**Compilação:**

```bash
gcc -Wall -Wextra -pedantic criptografia.c -o criptografia.exe
```

**Execução no Windows:**

```bash
.\criptografia.exe
```

**Execução no Linux ou macOS:**

```bash
gcc -Wall -Wextra -pedantic criptografia.c -o criptografia
./criptografia
```

## 8. Considerações Finais

O desenvolvimento deste projeto proporcionou a aplicação prática de conceitos fundamentais da programação em linguagem C.

A integração dos três módulos permitiu trabalhar com diferentes áreas da computação, desde algoritmos de criptografia e autenticação até simulações bancárias e processamento de imagens.

Além da implementação das funcionalidades, o projeto contribuiu para o desenvolvimento do raciocínio lógico, organização de código, tratamento de entradas, manipulação de arquivos e resolução de problemas.

É importante destacar que os mecanismos de criptografia utilizados possuem finalidade didática e não devem ser considerados adequados para proteger informações sensíveis em aplicações reais.

## 9. Desenvolvedor

**Antonio Dantas**

GitHub: [@AntonioADS06](https://github.com/AntonioADS06)

Projeto desenvolvido com finalidade acadêmica e educacional, utilizando a linguagem C para integração de funcionalidades e aplicação de conceitos de programação.

---

*Documentação técnica do projeto — Sistema Integrado em C.*
