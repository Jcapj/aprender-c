Progresso — Aprender C
Estado atual
Fase: 1 — Fundamentos (Fase 0 concluída em 2026-11-21)
Dia da rotina: próxima aula = dia 1 da semana 1 da Fase 1 (ler a parte nova do livro e digitar os exemplos)
Assunto atual: início da Fase 1, King cap. 2
Próxima atividade: aula 5 — King cap. 2: como a 2.1 já foi lida (bônus), revisar rapidamente o pun.c e seguir para a 2.2 (The General Form of a Simple Program), digitando os exemplos. Git da Fase 1: começar a usar git log e git diff
Pendências de critérios anteriores: nenhuma
Pendências de leitura: nenhuma (King cap. 1 e Seacord cap. 1 resolvidos em 2026-11-21)
Meu ambiente
Sistema: Windows 11 Home Single Language, versão 26H2 (build 26300.9974); virtualização habilitada; conta de administrador. WSL 3.0.5 com Ubuntu 26.04 LTS ("resolute"), usuário jose
Compilador e versão: gcc (Ubuntu 15.2.0-16ubuntu1) 15.2.0
Depurador: GNU gdb 17.1 (uso a partir da Fase 2)
Editor e extensões: VS Code 1.147.0 (x64), instalado no Windows com "Adicionar a PATH"; extensão WSL (ms-vscode-remote.remote-wsl) no Windows; extensão C/C++ (ms-vscode.cpptools 1.35.6) instalada no lado WSL: Ubuntu. Copilot não instalado e painel de Chat fechado (de propósito)
Git configurado: sim, em 2026-11-21 (user.name=JCAPJ, user.email=e-mail privado do GitHub 215318971+Jcapj@users.noreply.github.com, init.defaultBranch=main) | GitHub: conta Jcapj; autenticação por chave SSH ed25519 (~/.ssh/id_ed25519, sem passphrase, cadastrada como "Notebook WSL"); ssh -T git@github.com respondeu "successfully authenticated"
Ferramentas verificadas: gcc 15.2.0, gdb 17.1, valgrind 3.26.0, clang-format 21.1.8, git 2.53.0, make 4.4.1 (todas com --version em 2026-11-18); VS Code 1.147.0 (code --version) e extensões (code --list-extensions) em 2026-11-18
Pasta do curso: ~/aprender-c/fase0 (= /home/jose/aprender-c/fase0, dentro do Linux), aberta no VS Code com code . e marcada como confiável
Materiais: guia Guia_Aprender_C_v8.docx (a v8 só muda a descrição do King); King em PDF com texto legível e pesquisável (substituiu o escaneado)
Observação: ao abrir o Ubuntu, o WSL avisa "Falha ao configurar a rede (networkingMode Nat), voltando para networkingMode Consomme". A internet do Ubuntu funciona (apt update e apt upgrade concluídos).
Fases (anexo C do guia)
Fase	Início	Fim	Critério cumprido?	Projeto no GitHub	Observações
0	2026-11-18	2026-11-21	☑	☑	ficha.c (projeto) e receita.c (avaliação) no GitHub (github.com/Jcapj/aprender-c, fase0/). Avaliação sem consulta feita na aula 4
1			☐	☐	
2			☐	☐	
3			☐	☐	
4			☐	☐	
5			☐	☐	
6			☐	☐	
7			☐	☐	
Critério de saída da fase atual
Fase 1 (guia, seção 3):

☐ Resolve um problema simples do Beecrowd (laço + condição) em até 20 minutos.
☐ Explica a diferença entre int, float, double e char, incluindo a divisão inteira.
Fase 0 (cumprido em 2026-11-21, aula 4, sem consulta):

☑ Escreve, compila e roda um programa simples sem ajuda. (receita.c: nome de uma comida e 3 ingredientes, só printf, zero avisos)
☑ Entende a mensagem de um erro de compilação simples. (leu receita.c:4:5: error: implicit declaration of function 'printff'; did you mean 'printf'?: arquivo, linha 4, coluna 5, nome errado; consertou)
☑ Envia o código para o GitHub. (add/commit/push do PROGRESSO.md e do receita.c sozinho, com git status antes e depois)
Feito
Leituras: King cap. 1 completo ("Introducing C", p. 1–8; o capítulo não tem exercícios). Conferência em 2026-11-21: sabe que o C veio do B (Thompson) e foi criado por Ritchie nos Bell Labs para o UNIX (com ajuda); citou pontos fortes (portável, eficiente) e fracos (propenso a erros, difícil de ler), explicou em 2026-11-21: portável porque é padronizado (completamos: compiladores pequenos, disponíveis em quase todo computador); propenso a erros pela liberdade que dá (completamos: o compilador não detecta muitos erros); linguagem pequena, mas que combina recursos de jeitos confusos (ponto fraco "difícil de entender"). Pendência resolvida. Seacord cap. 1: Listagem 1-1 feita em aula; seção Function Return Values lida em 2026-11-21 (a puts pode falhar por erro de escrita da saída, não por erro no código; devolve EOF, negativo, se falhar e um valor não negativo se der certo; o programa deve conferir e terminar com EXIT_FAILURE, de <stdlib.h>. Ele acertou as duas primeiras e pediu a resposta da terceira). Bônus (Fase 1): King 2.1 lida, inclusive Compiling and Linking, Integrated Development Environments e Q&A sobre o GCC
Exercícios: Git (aula 3): git config, ssh-keygen, ssh -T, git init/status/add/commit/push, README.md. Bônus: pun.c (King 2.1) digitado; hello.c (Seacord, Listagem 1-1) digitado, compilado com gcc -std=c17 -Wall -Wextra -pedantic -g hello.c -o hello sem avisos e executado (Hello, world!); erro provocado de propósito (tirar o ;) e mensagem do gcc lida (arquivo:linha:coluna, setinha ^, olhar a linha anterior); terminal: pwd, ls, ls -la, mkdir, cd, cd .., cd ~
Projetos e repositórios: repositório público https://github.com/Jcapj/aprender-c (README.md, PROGRESSO.md na raiz e pasta fase0/ com hello.c, ficha.c e receita.c). Commits da aula 4: d03bee8 (PROGRESSO.md) e c360a48 (receita.c). Projeto da Fase 0 (ficha pessoal: nome, cidade, motivo; só printf, juntando textos entre aspas vizinhos) compilado com zero avisos e enviado: commit a0a8216. Obs.: pun.c não estava em fase0/ e não foi para o GitHub
Dificuldades
Ritmo: 1 hora por dia, de segunda a sexta (estudo extra conta como bônus). Experiência anterior com programação: praticamente zero.
Confundiu o prompt (~/aprender-c/fase0$) com um comando. Entendeu que o ~ é a pasta pessoal (/home/jose) e que para entrar numa pasta é preciso cd.
Prefere ir direto ao ponto: pediu para pular o experimento do a.out (o nome padrão sem -o, que ele acertou na teoria).
Na aula 3 pediu que eu fizesse a configuração do Git/GitHub por ele ("preguiça"). Fiz pelo navegador o que dava (cadastro da chave SSH e criação do repositório); o primeiro commit foi por um bloco colado. A ficha e o push dela ele fez digitando. Na avaliação, add/commit/push serão sem ajuda.
Fala por voz: às vezes a transcrição troca palavras ("boot" = Ubuntu, "PDF" = printf). Confirmar quando algo parecer estranho.
Comando de compilação: explicado peça por peça em 2026-11-21 (gcc, -std=c17 = padrão de 2017, -Wall, -Wextra, -pedantic, -g, arquivo.c, -o nome). Perguntou se podia usar -std=c23: combinado manter c17 até a Fase 5, como manda o guia.
Faz muitas perguntas de "por quê" (ótimo sinal). Em 2026-11-21 discutimos e ele explicou com as próprias palavras: return 0 × outros valores (recado de sucesso/falha para quem rodou o programa), #include e cabeçalhos (stdio.h, stdlib.h, biblioteca padrão × de terceiros), int main(void) × int main() (no C17 o void é o certo; no C23 os dois são iguais), argumentos da main (informação decidida por quem roda o programa; detalhes na Fase 3), diretivas # (pré-processador), as 3 etapas pré-processamento/compilação/linkagem, IDE × terminal.
Na aula 4 voltou a pedir a resposta em vez da dica (Seacord). Mesmo assim fez a avaliação inteira sozinho e saiu de vários erros lendo as mensagens.
Executáveis (ficha, hello, receita) ficam como "untracked" no git status: não vão para o repositório. Na Fase 1 criar o .gitignore.
Mensagens de commit: tende a escrever "Projeto da fase 0: ..." para tudo. Praticar mensagens que dizem o que o commit faz ("Adiciona receita.c").
Combinado: escrever no estilo do King (int main(void) e return 0;) e incluir só os cabeçalhos usados. Compilar sempre com o comando do guia, não com o do King (que usa -ansi, -W e -std=c99).
Caderno de erros
Data	O que deu errado	Por quê	Como resolvi
2026-11-18	Ao criar o usuário do Ubuntu: "Sorry, passwords do not match"	A senha não aparece na tela ao digitar no Linux, e as duas digitações ficaram diferentes	Li a mensagem, respondi y em "Try again?" e digitei a mesma senha duas vezes com atenção
2026-11-18	sudo apt install: "Unable to locate package valgrid" e depois "Unable to locate package gbd"	Erros de digitação nos nomes (valgrind, gdb). O apt precisa do nome exato e cancela o comando inteiro se um nome estiver errado	Li qual palavra a mensagem apontava, recuperei o comando com a seta ↑, corrigi e rodei de novo
2026-11-18	-bash: /home/jose/aprender-c/fase0$: No such file or directory	Digitei o caminho do prompt como se fosse comando: faltou o cd na frente, e o $ não faz parte do caminho (é só o fim do prompt)	Digitei cd ~/aprender-c/fase0
2026-11-18	gcc: ld: cannot find Wextra: No such file or directory	Escrevi Wextra sem o -. Sem o tracinho, o gcc trata a palavra como nome de arquivo, e o linker (ld) não acha esse arquivo; o executável não é criado	Comparei com o -Wall, coloquei o - (-Wextra) com a seta ↑ e compilei de novo, sem avisos
2026-11-18	(de propósito) hello.c:5:24: error: expected ';' before 'return'	Faltava o ; no fim da linha do puts; o gcc só percebe ao chegar no return da linha seguinte	Recoloquei o ;. Lição: ler arquivo:linha:coluna e, se a linha parecer certa, olhar a anterior
2026-11-21	ficha.c:3:12: error: missing terminating " character, seguido de 'Cidade' undeclared e stray '\' in program	Abri as aspas antes do nome e só fechei depois do motivo, com Enter no meio. Em C, as aspas que abrem e fecham têm que estar na mesma linha do código; quem pula linha na tela é o \n, não o Enter do editor	"Ou eu faço tudo numa linha só, ou cada parte tem a sua aspa aberta e a sua aspa fechada." Usei textos entre aspas vizinhos (o compilador junta). Lição: consertar sempre o primeiro erro, os outros vêm em cascata
2026-11-21	cc1: fatal error: ficha.c: No such file or directory	Compilei em ~/aprender-c, mas o arquivo está em ~/aprender-c/fase0. O gcc só procura na pasta atual	Olhei o prompt, fiz cd fase0 e compilei de novo
2026-11-21	-bash: cd~/aprender-c: No such file or directory (várias vezes)	Faltou o espaço entre cd e o caminho; o bash leu tudo como um comando só	Digitei cd ~/aprender-c, com espaço
2026-11-21	git push travou, sem resposta, e o que digitei depois (git status) não rodou	O push esperava a conexão com o GitHub (provavelmente a rede do WSL ainda acordando); enquanto o prompt não volta, o terminal não aceita comando novo	Ctrl+C para cancelar e git push de novo; funcionou
2026-11-21	gcc: error: -E or -x required when input is from standard input	Escrevi - pedantic com espaço; um - sozinho, para o gcc, quer dizer "ler o código do teclado"	Juntei: -pedantic
2026-11-21	receita: command not found	Para rodar um programa da pasta atual é preciso ./; sem ele o Linux procura um comando do sistema	./receita
2026-11-21	(avaliação) receita.c:4:5: error: implicit declaration of function 'printff'; did you mean 'printf'?	Nome da função escrito errado; printff não existe	Tirei um "f" (linha 4, coluna 5) e compilei de novo sem avisos
Histórico de aulas
2026-11-18 — Aula 1 (Fase 0): diagnóstico do computador; WSL 2 com Ubuntu 26.04 instalado; apt update/upgrade; build-essential, gdb, valgrind, clang-format e git instalados e verificados.
2026-11-18 — Aula 2 (Fase 0): VS Code 1.147.0 com extensões WSL e C/C++ (no WSL); terminal básico (pwd, ls, mkdir, cd); pasta ~/aprender-c/fase0; hello.c (Seacord 1-1) compilado sem avisos e executado; leitura de erros do gcc e do linker. Guia atualizado para a v8 e King trocado por PDF legível (sem mudança na Fase 0).
2026-11-21 — Sessão de dúvidas (Fase 0): return 0/1, cabeçalhos e biblioteca padrão, main(void) × main(), argumentos da main, diretivas #, etapas do gcc, IDEs; conferência parcial da leitura do King cap. 1; Seacord cap. 1 ficou como pendência.
2026-11-21 — Aula 3 (Fase 0): Git configurado; chave SSH criada e cadastrada no GitHub; repositório público aprender-c criado com README.md e fase0/; projeto da fase (ficha.c, só printf, zero avisos) escrito, compilado e enviado com add/commit/push.
2026-11-21 — Aula 4 (Fase 0): PROGRESSO.md enviado ao GitHub sozinho; Seacord cap. 1 (Function Return Values) resolvido; avaliação sem consulta: receita.c escrito, compilado sem avisos, erro printff lido e consertado, add/commit/push sozinho. Fase 0 concluída.