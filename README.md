# flexbox-e-grids

 ──────
   🧭 Guia Definitivo de Alinhamento no CSS

  Para qualquer alinhamento funcionar, o elemento pai precisa ter display: flex; ou display: grid;.
  ──────
  ## 1. Alinhamento no Eixo Horizontal (Direita, Esquerda, Espalhar)

  A propriedade mágica é justify-content:

   Comando                         │ O que faz visualmente?                                       │ Quando usar?
  ─────────────────────────────────┼──────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────
   justify-content: flex-start;    │ Gruda todo mundo na esquerda (início).                       │ Padrão do navegador.
   justify-content: flex-end;      │ Gruda todo mundo na direita (fim).                           │ Ícones no canto direito, botões de ação.
   justify-content: center;        │ Joga todo mundo no centro.                                   │ Menus de navegação, títulos.
   justify-content: space-between; │ Joga o primeiro na ponta esquerda, o último na ponta direita │ Seu caso do preço! (R$ 0 e R$ 250), cabeçalhos,
                                   │ e divide o espaço no meio.                                   │ títulos com ícone no canto.
   justify-content: space-around;  │ Dá o mesmo espaço ao redor de cada item.                     │ Cards espalhados com margens iguais.
   justify-content: space-evenly;  │ Espaço 100% rigorosamente igual entre todos e as bordas.     │ Menus bem distribuídos.
  ──────
  ## 2. Alinhamento no Eixo Vertical (Cima, Baixo, Centro)

  A propriedade principal é align-items:

   Comando                   │ O que faz visualmente?                               │ Quando usar?
  ───────────────────────────┼──────────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────
   align-items: center;      │ Centraliza na altura (ninguém fica mais alto/baixo). │ Alinhar logo com texto e ícones na mesma linha horizontal.
   align-items: flex-start;  │ Alinha tudo no topo.                                 │ Quando itens têm alturas diferentes e você quer alinhados por cima.
   align-items: flex-end;    │ Alinha tudo no fundo/chão.                           │ Alinhar preços ou botões pela base.
   align-items: stretch;     │ Estica os itens para terem a mesma altura.           │ Cards de produtos para ficarem todos com a mesma altura.
  ──────
  ## 3. Direção do Fluxo (Linha ou Coluna)

  A propriedade é flex-direction:

   Comando                                                                    │ O que faz?
  ────────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────
   flex-direction: row;                                                       │ Itens ficam lado a lado (horizontal - padrão).
   flex-direction: column;                                                    │ Itens ficam um embaixo do outro (vertical).
  ──────
  ## 4. Quebra de Linha

  A propriedade é flex-wrap:

   Comando                                                  │ O que faz?
  ──────────────────────────────────────────────────────────┼─────────────────────────────────────────────────────────────────────────────────────────────
   flex-wrap: nowrap;                                       │ Força todo mundo na mesma linha (padrão, pode esmagar).
   flex-wrap: wrap;                                         │ Se não couber na largura, pula para a linha de baixo (o que usamos nas bolinhas de cores!).
  ──────
  ## 5. Espaçamento entre Itens

  A propriedade é gap:

   Comando                                                                │ O que faz?
  ────────────────────────────────────────────────────────────────────────┼───────────────────────────────────────────────────────────────────────────────
   gap: 10px;                                                             │ Dá 10px de espaço entre todos os itens (tanto na horizontal quanto vertical).
   row-gap: 20px;                                                         │ Espaço só entre as linhas (vertical).
   column-gap: 15px;                                                      │ Espaço só entre as colunas (horizontal).
