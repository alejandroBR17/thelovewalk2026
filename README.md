# The Love Walk 2026 — Gerador de Molduras

![Prévia do The Love Walk 2026](og-preview.jpg)

Editor de imagens responsivo para a **Caminhada do Amor 2026**. Permite personalizar fotos com as molduras **Casados — NÓS VAMOS** e **Solteiros — EU VOU**, gerando imagens para perfil, Status/Stories e Feed.

**Site ao vivo:** https://thelovewalk2026.vercel.app

## Recursos

- Seleção inicial da moldura de **Casados** ou **Solteiros**.
- Escolha de **Perfil**, **Status** ou **Feed**, antes de enviar a foto; visualização imediata em cada formato.
- Uma única foto pode gerar os três formatos, sem precisar reenviá-la.
- Ajustes de posicionamento, zoom, pinça com dois dedos, rotação de 90° e enquadramento automático (detecção de rostos quando suportada).
- Fundo desfocado gerado a partir da própria foto, com controles de intensidade e escurecimento.
- Enquadramento e configurações preservados **individualmente para cada formato** quando o usuário alterna entre eles.
- Exportação **PNG**, botão de compartilhar pela API nativa do aparelho quando disponível e opção **Criar outro formato com esta foto**.
- Identidade visual roxa e laranja, ícones vetoriais e prévia Open Graph para compartilhamento do link.
- Processamento das fotos no navegador: **a imagem escolhida não é enviada ao servidor**.

## Formatos de saída

| Destino | Proporção | Resolução |
| --- | --- | --- |
| Foto de perfil | 1:1 | 1254 × 1254 px |
| Status do WhatsApp / Stories | 9:16 | 1080 × 1920 px |
| Feed do Instagram | 4:5 | 1080 × 1350 px |

As composições verticais acomodam a arte original em uma peça projetada na identidade do evento, **sem esticar ou recriar as molduras PNG**.

## Executar localmente

Este é um site estático feito em **HTML, CSS e JavaScript**, sem dependências de instalação ou back-end para editar fotos.

```bash
git clone https://github.com/alejandroBR17/thelovewalk2026.git
cd thelovewalk2026
python -m http.server 8000
```

Acesse `http://localhost:8000`. Você também pode abrir `index.html` diretamente, mas um servidor local evita possíveis restrições de carregamento de imagens do navegador.

## Arquivos

```text
.
├── index.html              # Site, interface e editor Canvas
├── assets/
│   ├── casados.png         # Moldura original: NÓS VAMOS
│   └── solteiros.png       # Moldura original: EU VOU
├── og-preview.jpg          # Imagem de compartilhamento do link
├── .gitignore
└── README.md
```

## Publicação

A versão pública está em **[thelovewalk2026.vercel.app](https://thelovewalk2026.vercel.app)**, na Vercel. Como o projeto é estático, os arquivos da raiz podem ser publicados por um serviço de hospedagem estática.

**Atenção:** este repositório contém uma cópia do código publicado; isso **não significa** que o projeto já esteja vinculado ao GitHub para deploy automático. Caso você conecte esse repositório ao projeto existente da Vercel, confirme a configuração de build e o domínio antes de ativar novas publicações.

## Créditos e uso das artes

Projeto desenvolvido para a divulgação do evento **The Love Walk 2026**. As artes de moldura pertencem ao material visual do evento; sua presença neste repositório **não concede licença de reutilização por terceiros**. Não foi definida uma licença geral para o projeto.
