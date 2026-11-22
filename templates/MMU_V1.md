# MMU — Frente baseada na referência visual de Davi (revisão 1.1)

**Status:** referência estrutural aprovada pelo usuário; coordenadas aproximadas ainda pendentes de homologação. **Branch:** feature/modelo-mestre-universal-v1.

## Referência recebida
Imagem enviada pelo usuário de 1199 × 1536 pixels (proporção ≈ 0,781). A imagem é a fonte visual de verdade para a **frente**. Não é autorização para alterar o verso. Não há arquivo de imagem versionado neste commit; manter a referência na conversa até sua incorporação técnica posterior.

## Hierarquia e composição observadas
1. Moldura dourada ornamental envolvendo a peça.
2. Topo: hexágono com coroa à esquerda, retrato cinematográfico de Davi ocupando a região superior esquerda; à direita, marca “Tesouros da Bíblia”, categoria “Reis e Guerreiros”, nome “DAVI” e subtítulo em fita.
3. Corpo: painel esquerdo com período, local e referências; coluna direita com três painéis (“Quem foi?”, “Qualidades”, “Lições”).
4. Pergaminho de lição principal no canto inferior esquerdo do corpo.
5. Faixa inferior de **LEGADO**, com ilustração temática, texto central e quatro destaques à direita. O legado é componente obrigatório da frente.

## Geometria preliminar normalizada (prancheta 1199 × 1536)
As caixas abaixo são aproximações de regiões visuais, não recortes exatos. O conteúdo ilustrado pode atravessar limites de regiões. Revisar com overlay antes de fixar coordenadas.

| Região | x | y | largura | altura |
|---|---:|---:|---:|---:|
| Moldura externa | 0 | 0 | 1199 | 1536 |
| Cabeçalho ilustrado | 20 | 15 | 1159 | 490 |
| Emblema | 30 | 35 | 185 | 195 |
| Marca e identificação | 590 | 20 | 510 | 470 |
| Painel período/local/referências | 30 | 520 | 460 | 430 |
| Painel Quem foi? | 505 | 505 | 660 | 185 |
| Painel Qualidades | 505 | 700 | 660 | 195 |
| Painel Lições | 505 | 905 | 660 | 285 |
| Pergaminho lição principal | 25 | 965 | 475 | 255 |
| Faixa Legado | 20 | 1210 | 1159 | 310 |

**Importante:** caixas aproximadas podem se sobrepor devido a adornos e composições orgânicas. Não aplicar teste de colisão retangular ingênuo a esses elementos.

## Invariantes
- Mesmo desenho de regiões, hierarquia e posições relativas para todas as categorias.
- Variáveis por personagem: retrato original, cenário, nome, subtítulo, período, local, referências, qualidades, lições e legado.
- Variáveis por categoria: paleta, emblema e ornamentação temática sem mudar a geometria-base.
- Texto deve ser fiel à Bíblia, com revisão editorial; não inventar dados ausentes.
- Não reutilizar imagens de jw.org ou wol.jw.org.
- O **verso** continua especificado separadamente e não foi redesenhado por esta referência.
- Sem merge, sem deploy, sem publicação.

## Próximas provas
1. Gerar overlay de linhas-guia sobre a imagem e refinar as coordenadas.
2. Verificar 25 pontos de alinhamento, margens e áreas de segurança.
3. Testar o encaixe com Rute e outros nomes/comprimentos de texto.
4. Homologar tipografia, legibilidade e exportação.

## Regra permanente: moldura externa oficial
A moldura dourada ornamental da primeira imagem de Davi enviada pelo usuário é obrigatória em todos os cards, frente e verso. Preservar contorno, ornamentos, cantos e proporções. Cores e emblemas internos podem variar por categoria, mas a moldura externa não pode ser substituída. A alternativa com gemas azuis foi rejeitada. Alterações exigem aprovação explícita. Cada card deve passar por comparação visual com a referência original antes da homologação.

## Regra de alinhamento do cabeçalho — referência DAVI
Na área direita do cabeçalho, definir o eixo vertical de composição pelo centro horizontal geométrico do texto **DAVI** no modelo original. Centralizar **horizontalmente nesse mesmo eixo** o título “TESOUROS DA BÍBLIA”, a categoria “REIS E GUERREIROS”, o nome do personagem e a faixa descritiva. Empilhar os elementos verticalmente com espaçamento visual equilibrado. O alinhamento vertical refere-se à organização da pilha, não a colocar todos os centros na mesma altura. Para outros nomes, adaptar escala tipográfica sem mover o eixo. Preservar retrato, hexágono e moldura oficial. Validar com overlay na imagem original antes de homologar coordenadas exatas.

## Regra permanente — emblemas hexagonais por categoria
A imagem de padronização de categorias enviada pelo usuário em 22/11/2026 é a referência visual normativa dos emblemas no cabeçalho superior. Todos compartilham moldura hexagonal dourada, proporção, posição e acabamento metálico. Símbolos e fundos: Reis e Guerreiros = coroa dourada sobre azul; Patriarcas e Líderes = tenda dourada sobre marrom; Profetas e Mensageiros = rolo dourado sobre cinza; Mulheres da Bíblia = lírio dourado sobre violeta; Apóstolos e Discípulos = espiga dourada sobre verde. Não substituir nem reinterpretar símbolos. O card de Davi conserva sua moldura externa original e o eixo de centralização do cabeçalho. Para produção, extrair ou redesenhar fielmente os emblemas a partir da referência fornecida pelo usuário, sem utilizar imagens de jw.org. Esta regra não autoriza merge ou deploy.
