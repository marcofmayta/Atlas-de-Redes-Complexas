# Atlas de Redes Complexas

**Entenda as redes e suas conexões.**

Um atlas interativo para explorar metodologias de redes complexas, acompanhar suas relações e consultar publicações científicas. O projeto reúne uma taxonomia navegável, um catálogo de dez artigos selecionados e diferentes visualizações que aproximam conceitos, técnicas e evidências bibliográficas.

## Acesse o atlas online

**[Abrir o Atlas de Redes Complexas](https://marcofmayta.github.io/Atlas-de-Redes-Complexas/)**

Acesse diretamente as três visualizações:

- **[Atlas principal](https://marcofmayta.github.io/Atlas-de-Redes-Complexas/)** — explore metodologias, publicações e ferramentas de pesquisa.
- **[Árvore metodológica — 10 artigos](https://marcofmayta.github.io/Atlas-de-Redes-Complexas/arvore_10_artigos.html)** — navegue pela hierarquia dos métodos associados aos artigos.
- **[Rede artigo–método — 10 artigos](https://marcofmayta.github.io/Atlas-de-Redes-Complexas/rede_10_artigos.html)** — visualize as conexões entre publicações e métodos.


## Sobre o projeto

Redes complexas aparecem em problemas de diferentes áreas, mas seus métodos nem sempre são fáceis de localizar ou relacionar. O Atlas de Redes Complexas foi criado para facilitar essa exploração: em vez de percorrer apenas uma lista de tópicos ou referências, o visitante pode navegar entre áreas metodológicas, abrir artigos e observar como os conceitos se conectam.

A página inicial oferece uma visão ampla do conteúdo. Duas visualizações complementares concentram-se nos **dez artigos selecionados**, mostrando somente os ramos e as relações metodológicas associados a essas publicações.

O atlas é uma ferramenta de exploração e consulta, não uma revisão sistemática nem um inventário exaustivo da literatura.

## O que você pode explorar

| Área | Recursos |
| --- | --- |
| **Metodologias** | Navegação por áreas, subáreas e técnicas, com cartões explicativos e acesso à taxonomia. |
| **Publicações** | Catálogo de dez artigos selecionados, informações bibliográficas, contribuições e links para as fontes. |
| **Mapa de relações** | Exploração visual de conexões entre métodos e publicações, com busca, seleção, filtros e controles de visualização. |
| **Ferramentas de pesquisa** | Recursos de aprendizado, matriz, comparação, caminhos, evolução, perguntas, biblioteca, curadoria e exploração dos dados. |
| **Árvore dos 10 artigos** | Hierarquia metodológica restrita aos ramos relacionados às dez publicações. |
| **Rede dos 10 artigos** | Grafo que conecta diretamente cada artigo aos métodos associados. |

## Três maneiras de navegar

### 1. Atlas principal — `index.html`

A porta de entrada do projeto. Apresenta as áreas metodológicas, publicações selecionadas, mapa de relações e ferramentas para investigar os vínculos entre os trabalhos. É o melhor ponto de partida para quem ainda não escolheu um tema.

Entre os recursos de navegação estão:

- Busca por métodos, títulos, autores e DOI.
- Cartões de áreas e tópicos metodológicos.
- Seleção de nós e consulta das respectivas relações.
- Filtros e controles de enquadramento dos mapas.
- Comparação e outros modos de exploração nas ferramentas de pesquisa.
- Exportação disponível em formatos como PNG, SVG e CSV, conforme a visualização.
- Atalhos de teclado e ajuda dentro da interface.

### 2. Árvore metodológica — `arvore_10_artigos.html`

Organiza os métodos em uma estrutura hierárquica e **exibe apenas os ramos vinculados às dez publicações**. Permite expandir ou recolher ramificações, pesquisar artigos ou métodos, recentrar a visualização e exportar o mapa em SVG.

Nos nós dos artigos, o **DOI aparece escrito na própria caixa**, acompanhado do botão **Abrir DOI**, que leva à página correspondente. Um painel complementar apresenta informações sobre o item selecionado.

### 3. Rede artigo–método — `rede_10_artigos.html`

Apresenta os dez artigos e os métodos relacionados como nós conectados em um grafo. É especialmente útil para perceber quais técnicas aparecem em diferentes trabalhos e investigar as relações de cada publicação.

A visualização inclui pesquisa, filtros por artigo e tipo de relação, seleção de nós, controles de navegação e exportação em SVG.

## Como usar

1. Acesse a **página inicial** e escolha uma área metodológica, uma publicação ou o mapa de relações.
2. Use a **busca** para localizar um conceito, um título, um autor ou um DOI.
3. Clique em um **nó ou cartão** para examinar as informações e conexões disponíveis.
4. Abra a **árvore metodológica** para seguir a hierarquia das técnicas presentes nos dez artigos.
5. Abra a **rede artigo–método** para comparar visualmente suas conexões.
6. Consulte os **links DOI** quando quiser chegar à fonte bibliográfica.

### Atalhos do Atlas principal

| Atalho | Ação |
| --- | --- |
| `/` ou `Ctrl + K` | Abrir a busca. |
| `Esc` | Fechar a pesquisa ou o painel ativo. |
| `Enter` | Ativar o nó selecionado. |

O zoom, o deslocamento do mapa e os demais controles também podem ser utilizados diretamente na interface.

## Interface e acessibilidade

O projeto usa uma interface adaptável a telas de computador e dispositivos móveis. As transições, conexões animadas, efeitos de profundidade e respostas à interação ajudam a orientar a exploração, sem substituir os controles de navegação.

Há suporte a preferências de movimento reduzido e, na página principal, um controle para pausar animações. Os elementos interativos incluem rótulos e estados de foco para favorecer a navegação por teclado.

## Estrutura do repositório

```text
Atlas-de-Redes-Complexas/
├── index.html                 # Página principal e atlas completo
├── arvore_10_artigos.html     # Árvore metodológica dos dez artigos
├── rede_10_artigos.html       # Rede entre artigos e métodos
└── README.md                  # Documentação do projeto
```

As três páginas HTML funcionam de maneira independente e estão conectadas por links de navegação. Para que os links relativos funcionem corretamente, mantenha os arquivos HTML na mesma pasta, com os nomes acima.

## Executar localmente

Você pode abrir `index.html` diretamente no navegador. Para desenvolvimento e testes, também é possível iniciar um servidor local na pasta do projeto:

```bash
git clone https://github.com/marcofmayta/Atlas-de-Redes-Complexas.git
cd Atlas-de-Redes-Complexas
python -m http.server 8000
```

Depois, acesse **http://localhost:8000**.

O projeto utiliza HTML, CSS e JavaScript, com visualizações SVG interativas. As páginas foram distribuídas como arquivos HTML autossuficientes, sem necessidade de instalar pacotes ou executar uma etapa de compilação para visualizar o conteúdo.

## Publicar no GitHub Pages

1. Envie `index.html`, `arvore_10_artigos.html`, `rede_10_artigos.html` e `README.md` para a raiz do repositório.
2. No GitHub, abra **Settings → Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**.
4. Selecione a branch principal e a pasta **/(root)** e salve.
5. Acesse o endereço publicado após a conclusão da implantação.

Endereço do projeto: **https://marcofmayta.github.io/Atlas-de-Redes-Complexas/**

## Escopo e interpretação

As conexões indicam as associações metodológicas documentadas no conjunto de publicações selecionado. A presença de uma ligação não significa, por si só, que dois artigos compartilham os mesmos resultados, que um método supera outro ou que exista uma relação causal entre eles.

Da mesma forma, **a ausência de um tópico nos mapas especializados não significa que ele não faça parte do campo de redes complexas**: nesses mapas, somente os métodos associados aos dez trabalhos foram incluídos.

Para avaliações científicas, recomenda-se consultar os artigos originais e examinar o contexto em que cada método foi empregado ou discutido.

## Autor

**Marco Mayta**

Desenvolvimento e organização do Atlas de Redes Complexas.

[GitHub](https://github.com/marcofmayta) · [Repositório](https://github.com/marcofmayta/Atlas-de-Redes-Complexas)
