# Painel iGov-Jus

**Índice Amplo de Governança da Justiça**

🔗 **Painel publicado:** https://marcelojustus.github.io/painel.iGov-Jus/

O Painel iGov-Jus é uma plataforma interativa de visualização de dados que reúne indicadores de **produtividade, transparência, governança de TIC e eficiência** dos **27 Tribunais de Justiça estaduais** do Brasil. Os rankings, as séries temporais, o mapa e as tabelas permitem comparar o desempenho institucional dos tribunais a partir de uma perspectiva mais ampla do que a da produtividade processual tradicional.

> **Escopo da primeira etapa.** Nesta etapa, o projeto contempla apenas a **Justiça Estadual**. As demais esferas do Poder Judiciário poderão ser incorporadas em etapas posteriores.

---

## Sumário

- [Contexto e motivação](#contexto-e-motivação)
- [O índice iGov-Jus](#o-índice-igov-jus)
- [Funcionalidades do painel](#funcionalidades-do-painel)
- [Dados e fontes](#dados-e-fontes)
- [Notas metodológicas](#notas-metodológicas)
- [Como utilizar](#como-utilizar)
- [Como citar](#como-citar)
- [Equipe](#equipe)
- [Limitações e avisos](#limitações-e-avisos)

---

## Contexto e motivação

O Poder Judiciário brasileiro é um dos mais custosos em perspectiva comparada. Segundo o *Justiça em Números 2025* (CNJ, 2025), em 2024:

| Indicador | Valor |
|---|---|
| Despesas totais do Judiciário | R$ 146,5 bilhões (1,2% do PIB) |
| Novos processos ingressados | 39,4 milhões |
| Processos baixados | 44,8 milhões |
| Processos pendentes ao final do ano | 80,6 milhões |
| Taxa de congestionamento | 64,3% (menor patamar em 16 anos) |

O projeto parte da premissa de que as disfunções do Judiciário não decorrem apenas do excesso de processos ou da escassez de recursos, mas constituem, sobretudo, **um problema de governança pública**, no qual incentivos, regras institucionais, capacidade administrativa, transparência, *accountability* e padrões de litigiosidade interagem para determinar a eficiência, a eficácia e a efetividade da prestação jurisdicional. O referencial teórico dialoga com a nova economia institucional (North; Williamson; Ostrom), com a literatura de administração pública (Rhodes; Hood; Osborne; Pollitt & Bouckaert), com a análise econômica do direito (Gico Jr.; Cooter & Rubinfeld) e com o modelo de governança judicial de Akutsu e Guimarães (2015).

Nesse contexto, discute-se criticamente o **IPC-Jus**, índice de produtividade comparada utilizado pelo CNJ para ranquear tribunais, sob o argumento de que uma justiça de qualidade não pode ser confundida apenas com uma justiça rápida ou quantitativamente produtiva. O iGov-Jus propõe, assim, um indicador de desempenho capaz de captar aspectos mais amplos da governança judicial.

## O índice iGov-Jus

O iGov-Jus é estruturado em **cinco dimensões complementares**:

| # | Dimensão | Origem | Descrição |
|---|---|---|---|
| 1 | **IPC-Jus** | CNJ | Índice de Produtividade Comparada: mede a produtividade relativa dos tribunais. |
| 2 | **ITP-Jus**¹ | CNJ | Pontuação do Ranking da Transparência do Poder Judiciário: publicidade institucional e *accountability*. |
| 3 | **iGovTIC-JUD** | CNJ | Índice de Governança, Gestão e Infraestrutura de Tecnologia da Informação e Comunicação do Poder Judiciário. |
| 4 | **EGAG-Jus** | Este estudo | Indicador de Eficiência Relativa do Acesso à Justiça e da Gestão da Demanda Judicial: avalia a capacidade de administrar pressão processual, congestionamento e tempo de tramitação diante das restrições organizacionais e dos custos da assistência judiciária gratuita. |
| 5 | **EGFP-Jus** | Este estudo | Indicador de Eficiência Relativa da Gestão do Fluxo Processual: avalia a capacidade de converter recursos organizacionais e de administrar pressões associadas à litigiosidade, à assistência judiciária gratuita e à recorribilidade em menores níveis de congestionamento. |

¹ "ITP-Jus" é uma abreviação adotada neste estudo para a pontuação do Ranking da Transparência do Poder Judiciário, do CNJ. **Não se trata de um índice oficial do CNJ.**

## Funcionalidades do painel

O painel é organizado nas seguintes seções:

- **Metodologia** — apresentação do referencial teórico, do escopo e da construção do índice.
- **Rankings** — classificação dos tribunais por indicador e ano.
- **Séries temporais** — evolução dos indicadores ao longo do tempo, com opção de suavização por média móvel.
- **Correlações** — matriz de correlação linear de Pearson entre os indicadores (variáveis originais do IPC-Jus e componentes do iGov-Jus em 2024).
- **Dispersão** — gráficos de dispersão com seleção de eixos X e Y, tamanho dos pontos, ano, reta de ajuste linear e R².
- **Comparação de índices** — confronto entre dois índices, com tribunais ordenados pelo primeiro e indicação das posições em 2024.
- **Mapa** — visualização geográfica por unidade da federação, com cores e bolhas; estados sem dados aparecem em cinza.
- **Distribuição** — distribuição dos indicadores em *z-score* (2024), com a normal teórica N(0,1) como referência.
- **Dados** — tabela pesquisável, com opção de **download em CSV**.
- **Equipe** — apresentação dos pesquisadores responsáveis.

### Filtros e opções de exibição

- Seleção por **porte do tribunal** (grande, médio e pequeno) ou tribunal a tribunal;
- Opções de "marcar todos" e "desmarcar todos";
- Alternância entre valores originais e **z-score**;
- Seleção de indicador e de ano.

## Dados e fontes

- **Fonte principal:** Conselho Nacional de Justiça (CNJ). *Justiça em Números 2025*. Disponível em: <https://www.cnj.jus.br/pesquisas-judiciarias/justica-em-numeros/>.
- **Cobertura:** 27 Tribunais de Justiça estaduais.
- **Disponibilidade temporal:** os indicadores ITP-Jus, iGovTIC-JUD, EGAG-Jus, EGFP-Jus e iGov-Jus estão disponíveis **apenas para 2024**.

## Notas metodológicas

- **Eficiência relativa (DEA).** Diferentemente do CNJ, este estudo inclui o **tamanho da população como *input*** no modelo de Análise Envoltória de Dados (DEA). O IPC-Jus modificado reflete essa especificação.
- **Tratamento dos processos.** Excluem-se processos suspensos, execuções fiscais e execuções penais.
- **Tratamento das despesas.** As despesas são deflacionadas pelo IPCA (base 2024).
- **Padronização.** A exibição em *z-score* permite comparar indicadores de escalas distintas.
- **Correlações.** Calculadas pelo coeficiente linear de Pearson.

## Como utilizar

O painel é uma página estática, acessível diretamente pelo navegador, sem necessidade de instalação:

👉 https://marcelojustus.github.io/painel.iGov-Jus/

> Os gráficos, o mapa e as tabelas interativas exigem **JavaScript habilitado**.

Navegação em dispositivos com tela sensível ao toque, como celulares e tablets, basta arrastar a tela para o lado para alternar entre as páginas do painel.

## Como citar

Sugestão de citação:

> JUSTUS, Marcelo; TIMM, Luciano Benetti; GERALDINI, Bernardo; RODRIGUES, Luis Felipe de Souza. **Painel iGov-Jus: Índice Amplo de Governança da Justiça** (primeira etapa: Justiça Estadual). 2026. Disponível em: https://marcelojustus.github.io/painel.iGov-Jus/. Acesso em: __ de ______ de ____.

Ao utilizar os dados do CNJ, cite também: CONSELHO NACIONAL DE JUSTIÇA. *Justiça em Números 2025*. Brasília: CNJ, 2025.

## Equipe

| Nome | Função | Afiliação |
|---|---|---|
| **Marcelo Justus** | Coordenação | Instituto de Economia, Unicamp |
| **Luciano Benetti Timm** | Coordenação Adjunta | IDP, São Paulo |
| **Bernardo Geraldini** | Pesquisa | Instituto de Economia, Unicamp |
| **Luis Felipe de Souza Rodrigues** | Apoio à pesquisa | Mestre em Economia (UFMT) e Cientista de dados |

## Limitações e avisos

- O painel tem **finalidade acadêmica e informativa**; os indicadores não constituem avaliação oficial do CNJ nem de qualquer tribunal.
- A primeira etapa abrange somente a Justiça Estadual.
- Parte dos indicadores está disponível apenas para o ano de 2024, o que limita análises longitudinais.
- Os resultados dependem das escolhas metodológicas descritas acima, em especial a especificação do modelo DEA.

## Principais Referências

- AKUTSU, L.; GUIMARÃES, T. A. Governança judicial: proposta de modelo teórico-metodológico. *Revista de Administração Pública*, v. 49, n. 4, p. 937–958, 2015.
- CONSELHO NACIONAL DE JUSTIÇA. *Justiça em Números 2025*. Brasília: CNJ, 2025.
- GICO JR., I. T. A tragédia do Judiciário. *Revista de Direito Administrativo*, v. 267, p. 163–198, 2014.
- NORTH, D. C. *Institutions, Institutional Change and Economic Performance*. Cambridge University Press, 1990.
- WILLIAMSON, O. E. *The Mechanisms of Governance*. Oxford University Press, 1996.

A lista completa de referências encontra-se na seção de Metodologia do painel.

---

## Participe

O Painel iGov-Jus é um projeto em constante aprimoramento e recebe com interesse contribuições e comentários da comunidade. Seja você pesquisador, magistrado, servidor de tribunal, gestor público ou profissional que atua com governança, transparência e eficiência do sistema de justiça, sua colaboração é muito bem-vinda para o desenvolvimento de indicadores mais consistentes e úteis à sociedade.

Sinta-se à vontade para explorar o painel, consultar a seção de Metodologia, sugerir melhorias, apontar inconsistências nos dados ou propor novas dimensões de análise. As contribuições podem ser enviadas por meio das *issues* do repositório ou pelos canais de contato indicados neste documento.

Agradecemos o seu interesse no iGov-Jus. Juntos, podemos fortalecer a governança do Poder Judiciário e ampliar a transparência e a qualidade da prestação jurisdicional no Brasil.

## Agradecimentos

Os coordenadores do projeto iGov-Jus expressam seu reconhecimento ao Instituto [Convergência Brasil](https://convergenciabrasil.com/) pelo apoio financeiro destinado à elaboração de um policy paper, que constituiu a base conceitual para a formulação da proposta do iGov-Jus.

## Financiamento e independência institucional

O projeto iGov-Jus não dispõe, atualmente, de financiamento público ou privado. Sua concepção, desenvolvimento e execução são conduzidos de forma independente, sob a responsabilidade exclusiva de seus coordenadores. O projeto não possui vinculação institucional com as organizações às quais seus coordenadores estão vinculados, tampouco representa posições ou manifestações oficiais dessas instituições.

## Licença

[Painel iGov-Jus: Índice Amplo de Governança da Justiça](https://marcelojustus.github.io/painel.iGov-Jus/) © 2026 por [Marcelo Justus](https://www.marcelojustus.com/) está licenciado sob [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/).
 
<a href="https://creativecommons.org/licenses/by-nc-nd/4.0/"><img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nc.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"><img src="https://mirrors.creativecommons.org/presskit/icons/nd.svg" alt="" style="max-width: 1em;max-height:1em;margin-left: .2em;"></a>
 
Em termos gerais, a licença permite copiar e redistribuir o material em qualquer meio ou formato, desde que (i) seja dado o devido crédito, (ii) não haja uso comercial e (iii) o material **não seja modificado ou adaptado** para distribuição.
 
**Dados de terceiros.** A licença abrange apenas a criação original do projeto (índices EGAG-Jus e EGFP-Jus, visualizações, textos e base derivada). Os dados originais do *Justiça em Números* pertencem ao CNJ e seguem as condições de uso estabelecidas por esse órgão.
