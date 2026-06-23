<img width="2480" height="254" alt="Cabecalho 3" src="https://github.com/user-attachments/assets/14f721de-0601-4f8d-9782-06dc02ec0d44" />

# Projeto final: Jogo da forca
Heloísa Fernandes Cano - Ilum Escola de Ciência (CNPEM) <br>
Turma 26 - 1° Semestre - Práticas em Ciência de Dados

Esse projeto corresponde ao projeto final da disciplina de Práticas em Ciência de Dados, ministrada pelos professores doutores Daniel Roberto Cassar, James Moraes de Almeida e Leandro Nascimento Lemos, no 1° semestre do ano de 2026.

## Descrição
O projeto consiste em uma implementação do tradicional jogo da forca, utilizando a linguagem de programação <b>Python</b> para elaboração dos códigos e a biblioteca integrada <b>Tkinter</b> para o desenvolvimento da interface gráfica do projeto.
Nele, o jogador escolhe uma <b>dificuldade</b>, que determina a <u>quantidade de erros que um jogador pode cometer</u>, e um <b>tema</b>, do qual a palavra será sorteada. O objetivo do jogo é descobrir a palavra misteriosa, chutando letra por letra, antes de atingir o limite de erros permitido!

## Funcionalidades
- Interface gráfica desenvolvida com Tkinter;
- Seleção de dificuldade;
- Seleção de tema;
- Sorteio aleatório de palavras;
- Controle de acertos e erros;
- Suporte a letras acentuadas e cedilha;
- Reinício da partida;
- Tela de vitória e derrota.

## Como executar?
1. Clone esse repositório:
   ```git clone https://github.com/helocano/jogo-da-forca.git```
   
2. Acesse a pasta do projeto:
   ```cd jogo-da-forca```

3. Execute o arquivo ```forca_index.ipynb```

## Regras & Passo a Passo
- O jogador escolhe uma dificuldade, dentre Fácil, Médio, Difícil ou Impossível.
  - Fácil: 15 erros
  - Médio: 7 erros
  - Difícil: 5 erros
  - Impossível: 0 erros
- O jogador escolhe um tema, dentre animais, comidas, elementos, ilum, países, pokémon, profissões ou verbos
  - Animais: Mais de 290 animais possíveis, dentre mamíferos, aves, répteis, peixes, etc
  - Comidas: Mais de 150 comidas diferentes
  - Elementos: Todos os 118 elementos da tabela periódica
  - Ilum: Mais de 90 palavras possíveis, dentre professores e disciplinas
  - Países: Mais de 190 países diferentes
  - Pokémon: 251 pokémon, abrangendo as regiões de Kanto e Johto
  - Profissões: Mais de 240 profissões diferentes
  - Verbos: 150 verbos diferentes
- Dentro do tema escolhido, uma palavra é sorteada aleatoriamente.
- O jogador digita as letras que ele acredita ter na palavra:
  - Letras corretas são reveladas em suas respectivas posições
  - Letras erradas aumentam o contador de erros
  - Tem muita certeza de qual é a palavra? Digite-a no campo de letras para chutar! Mas cuidado: se o seu chute estiver errado, o jogo acaba imediatamente!
- O jogo termina quando:
  - todas as letras forem adivinhadas;
  - a palavra misteriosa foi descoberta;
  - o limite de erros é atingido.
- Divirta-se!
  
## Decisões de Implementação
- O estado da partida é armazenado em um único dicionário chamado `estado_jogo`.
- As palavras são carregadas a partir de arquivos `.txt` organizados por tema.
- Letras acentuadas são tratadas como equivalentes às suas versões sem acento.
- A interface foi desenvolvida inteiramente com Tkinter.

## Implementações Futuras
- Botão de instruções dentro do jogo
- Opção de pedir dica para adivinhar a palavra
- Contador de vitórias consecutivas
- Utilizar a dificuldade como filtro de palavras, e não apenas limite de erros
- Opção de criar os próprios temas e palavras
- Adições de elementos visuais representativos
