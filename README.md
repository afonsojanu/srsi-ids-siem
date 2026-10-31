# Integração entre IDS e SIEM

**Segurança em Redes e Sistemas de Informação · Projeto — Parte 1**  
Mestrado em Engenharia Informática · Iscte — Instituto Universitário de Lisboa

Revisão da literatura sobre a eficácia da integração entre sistemas de deteção de intrusões e plataformas de gestão e correlação de eventos de segurança em redes empresariais. A síntese reúne **18 estudos**, comparando configurações, resultados, qualidade da evidência e limitações.

**[Ler o relatório](projeto.pdf) · [Consultar os 18 artigos](artigos/README.md) · [Ver a extração dos estudos](dados/extracao-18-estudos.csv) · [Aceder às fontes LaTeX](latex/)**

## O que investigamos

O trabalho analisa em que condições a integração IDS–SIEM contribui para a deteção de ataques. Distingue três intervenções que nem sempre são separadas nos estudos: centralizar alertas, acrescentar sensores e correlacionar fontes de contexto.

A evidência analisada sustenta benefícios de contexto e de funcionamento em determinadas configurações, mas não permite atribuir uma melhoria universal de deteção apenas à presença de um SIEM. Os comparadores, as unidades de análise e os denominadores das métricas são essenciais para interpretar os resultados.

## Materiais disponíveis

| Localização | Conteúdo |
| --- | --- |
| [projeto.pdf](projeto.pdf) | Relatório com fundamentação, metodologia, comparação dos 18 estudos, discussão, conclusões e trabalhos futuros. |
| [latex/](latex/) | Texto, capa, bibliografia, imagens e gráficos necessários para compilar o relatório. |
| [artigos/](artigos/) | Catálogo dos 18 estudos, referências BibTeX, ligações às fontes e três PDFs com licença de redistribuição confirmada. |
| [dados/](dados/) | Extração dos estudos e decisões da reformulação da seleção. |
| [parsifal/](parsifal/) | Exportações da revisão, estados de seleção, campos de extração e contagens dos gráficos. |
| [pesquisas/](pesquisas/) | Expressões e registos de pesquisa, exportações bibliográficas originais e reconciliação documental. |

O repositório é público e pode ser consultado sem autenticação. Para descarregar os materiais, utilizar **Code → Download ZIP**. Esse ZIP do GitHub contém a documentação completa do repositório; o ZIP submetido na plataforma da cadeira contém apenas as fontes necessárias para compilar o relatório.

## Como consultar a revisão

1. Ler o [relatório](projeto.pdf), começando pela pergunta de investigação e pela metodologia.
2. Comparar os estudos na tabela de síntese e consultar os resultados e limites de interpretação.
3. Usar os identificadores dos estudos, como `P02` ou `A058`, para localizar a respetiva entrada no [catálogo](artigos/README.md) e na [extração](dados/extracao-18-estudos.csv).
4. Consultar os apêndices e os registos de pesquisa para compreender as contagens, as decisões de seleção e as limitações de reprodução.

## Compilar o relatório

Abrir `latex/main.tex` e utilizar **XeLaTeX** com **BibTeX**, mantendo a estrutura das pastas.

```sh
cd latex
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

No Overleaf, carregar o conteúdo de `latex/`, definir `main.tex` como documento principal e selecionar XeLaTeX. A compilação também foi verificada com Tectonic.

## Âmbito e interpretação

A revisão tem âmbito delimitado e não representa uma cobertura exaustiva da literatura. Os critérios da seleção focalizada foram definidos após a avaliação inicial; as limitações históricas de pesquisa e a ausência de validação independente estão explicitadas no relatório. As contagens de registos importados não devem ser confundidas com os **18 estudos incluídos**.

As experiências dos artigos não foram reproduzidas neste projeto teórico. A secção de trabalhos futuros propõe condições comparáveis para a fase prática, com recall, precisão, F1, taxa de falsos positivos e medidas de latência.

## Artigos e direitos de utilização

Os artigos pertencem aos respetivos autores e titulares de direitos. As licenças e as fontes dos três PDFs disponibilizados encontram-se no [catálogo de artigos](artigos/README.md). Para os restantes estudos são fornecidas ligações; algumas podem exigir acesso institucional. Não se aplica uma licença única aos artigos de terceiros.

## Grupo

- Afonso Miguel Teixeira Januário
- João Pedro Cravinho Dias
- Sérgio Grubleac Silva
- Wandir Etiene Louro Moreira de Castro

**Docente:** Valderi Reis Quietinho Leithardt  
**Unidade curricular:** Segurança em Redes e Sistemas de Informação  
**Ano:** 2026
