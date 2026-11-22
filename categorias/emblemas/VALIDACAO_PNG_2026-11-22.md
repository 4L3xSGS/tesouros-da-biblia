# Validação PNG e prova de cabeçalhos — 22/11/2026

## Verificação de integridade
Os cinco arquivos da branch foram confrontados com cópias locais, usando o SHA-1 de objeto blob do Git (`sha1("blob "+size+"\\0"+bytes)`). Todos coincidem com os SHA retornados pela API do GitHub.

| Arquivo | Bytes | Git blob SHA | Dimensão | Modo |
|---|---:|---|---|---|
| reis-guerreiros.png | 520596 | 8c53309d4c463718062354b761a516f9263aa410 | 752×752 | RGBA |
| patriarcas-lideres.png | 520123 | a905cb3c220f63cf8eb837061fdad26f252b8e8f | 752×752 | RGBA |
| profetas-mensageiros.png | 492771 | 142becdb5197c8e0bcce5d41e7af4efb09840440 | 752×752 | RGBA |
| mulheres-biblia.png | 571095 | 2f64e211b82c83fa240db09cfcd6d377e06ea43d | 752×752 | RGBA |
| apostolos-discipulos.png | 510077 | 86593a4d3f535f2f1916a86b58ba59fd15b4eb81 | 752×752 | RGBA |

Canal alfa presente nos cinco, intervalo de valores 0–255. Proporção de pixels aproximadamente: 68% opacos, 24,4% transparentes, 7,6% parcialmente transparentes. Isso confirma transparência, mas não homologa qualidade visual das bordas.

## Prova visual
Foi preparada uma composição técnica lado a lado de dois cabeçalhos, utilizando o recorte da frente original de Davi e sobrepondo os **PNGs reais** de coroa e lírio no mesmo slot. O painel Rute é um placeholder de posicionamento: não representa retrato, textos ou card final de Rute. A prova foi entregue como arquivo na conversa, **não versionado neste repositório**.

Foi produzida também uma ilustração conceitual separada; seus emblemas não são os arquivos oficiais e não devem ser usados para homologação.

## Resultado
**PASSA:** presença no GitHub, correspondência exata de bytes, dimensão, decodificação RGBA e canal alfa.

**PENDENTE:** qualidade do recorte nas bordas, fidelidade visual pixel a pixel, escala no cabeçalho, substituição real dos demais conteúdos de Rute, alinhamento tipográfico, revisão de moldura e aprovação humana.

Sem merge nem deploy.
