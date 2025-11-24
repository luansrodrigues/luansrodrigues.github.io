# Imagens dos Posts

Este diretório contém as imagens usadas nos posts do blog.

## Estrutura

Coloque as imagens dos posts neste diretório: `themes/tech-blog-theme/static/images/posts/`

## Como usar

### 1. Imagem Principal do Post (Open Graph)

No front matter do post, adicione:
```yaml
image: "/images/posts/nome-da-imagem.png"
```

Esta imagem será:
- Exibida no topo do post
- Usada para compartilhamento social (Open Graph/Twitter Cards)
- Recomendado: 1200x630px

### 2. Imagens no Conteúdo

No conteúdo markdown do post, use:
```markdown
![Descrição da imagem](/images/posts/nome-da-imagem.png)
```

## Imagens de Exemplo Adicionadas

Os seguintes posts têm referências a imagens (você precisa adicionar as imagens reais):

- `blockchain-osint-guide.png` - Post: Como começar em Blockchain OSINT
- `bitcoin-tracking.png` - Post: Como rastrear uma carteira no Bitcoin
- `blockchain-explorer.png` - Imagem no conteúdo do post sobre Bitcoin
- `bitcoin-transaction-graph.png` - Grafo de transações no post sobre Bitcoin
- `ethereum-mapping.png` - Post: Mapeando transações no Ethereum
- `etherscan-interface.png` - Interface do Etherscan no conteúdo
- `smart-contract-analysis.png` - Análise de contrato no conteúdo
- `breadcrumbs-tutorial.png` - Post: Introdução ao Breadcrumbs
- `breadcrumbs-visualization.png` - Visualização no conteúdo

## Gerar Imagens

Você pode usar o script para gerar imagens Open Graph:
```bash
python3 scripts/generate_og_image.py "Título" "Descrição" themes/tech-blog-theme/static/images/posts/nome.png
```

## Formatos Recomendados

- **Formato**: PNG ou JPG
- **Tamanho Open Graph**: 1200x630px
- **Imagens no conteúdo**: Qualquer tamanho (serão redimensionadas automaticamente)
- **Otimização**: Comprima as imagens antes de adicionar (use ferramentas como TinyPNG)

