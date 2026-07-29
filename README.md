# Sweet Sketch, Unipessoal Lda — proposta de website

Proposta de website em duas versões para a **Sweet Sketch, Unipessoal Lda**, construtora sediada em Grândola.
Produzido pela [Elevia Digital](https://elevia.pt).

Publicado em `https://elevia.pt/sweet-sketch/` (Hostinger).

## O cliente

| | |
|---|---|
| Nome | Sweet Sketch, Unipessoal Lda |
| NIF | 516997904 |
| Sede | Grândola, distrito de Setúbal |
| Constituída | maio de 2022 |
| CAE | 41000, construção de edifícios residenciais e não residenciais |

Faz construção de edifícios, remodelações e pinturas, instalações elétricas, canalizações e redes de fluídos, climatização, telecomunicações e segurança, carpintaria, caixilharia e coberturas, estucagem, revestimentos, demolição e preparação de terreno. Tem ainda atividade imobiliária: compra e venda, arrendamento, mediação e administração de imóveis.

## Estrutura

```
index.html      página única, sem dependências, com três vistas
img/            fotografias e ficheiros do logótipo
marca/          kit do logótipo para uso fora do site
```

O `index.html` é uma página única que carrega diretamente o site (versão completa). Secções, por ordem:

1. **Hero** — carrossel de especialidades
2. **01 / Especialidades** — serviços
3. **02 / Portefólio** — 12 obras filtráveis (imagens ilustrativas)
4. **03 / Obras recentes** — **fotografias reais**, filtráveis por categoria
5. **04 / Antes e depois** — comparador interativo
6. **05 / Como trabalhamos** — processo
7. **06 / Clientes** — testemunhos (exemplo)
8. **07 / Artigos** — 3 artigos, cada um com uma nota expansível de ajuda
9. **08 / Pedir orçamento** — formulário e contactos

A secção **Obras recentes** (`RECENTES`) é a única com **fotografias reais** das obras da Sweet Sketch. Está organizada por categoria (`RECFILTROS`): Madeiras, Isolamentos, Microcimentos, Coberturas e Pladur. Mostra primeiro um cartão-capa por categoria (imagem ilustrativa + contagem); ao clicar, abre a galeria masonry dessa categoria, com lightbox que navega só dentro dela e um botão "Todas as categorias" para voltar. O portefólio acima ainda usa imagens ilustrativas.

Cada artigo (`ARTIGOS`) tem um campo `nota` com HTML de ajuda, mostrado num `<details>` "Saber mais".

Todo o restante conteúdo é gerado a partir de tabelas de dados no topo do `<script>` (`SLIDES`, `SERVICOS`, `OBRAS`, `RECENTES`, `PROCESSO`, `TESTS`, `ARTIGOS`, `MARQUEE`). Para mudar textos ou fotografias, edite essas tabelas, não o HTML.

## Publicar na Hostinger

1. hPanel, Gestor de Ficheiros
2. Entrar em `public_html/sweet-sketch/`
3. Carregar `index.html` e a pasta `img/`, confirmando a substituição

Não é preciso build nem instalar nada. A única dependência externa é o Google Fonts (Archivo e JetBrains Mono).

## Logótipo

O logótipo foi extraído do original enviado pelo cliente (JPEG com fundo escuro) e recortado com transparência. Existe em quatro composições:

- `logo-claro.png` / `logo-escuro.png` — lockup empilhado, marca sobre o nome e "CONSTRUTORA"
- `logo-h-claro.png` / `logo-h-escuro.png` — lockup horizontal, usado nas barras de navegação e rodapés
- `marca-clara.png` / `marca-escura.png` — só o símbolo

"Claro" e "escuro" referem-se à **cor da arte**, não ao fundo: use `logo-claro` sobre fundos escuros e `logo-escuro` sobre fundos claros.

## Por preencher

O site está marcado como demonstração porque parte do conteúdo é de exemplo. Falta pedir ao cliente:

- [ ] Telefone, email e morada exata
- [ ] Número de alvará
- [x] Fotografias de obras reais — 18 fotografias na secção "Obras recentes" (o portefólio de cima continua ilustrativo)
- [ ] Testemunhos de clientes
- [ ] Números concretos: obras concluídas, m² construídos, dimensão da equipa
- [ ] Confirmar as promessas "resposta em 24 horas" e "visita técnica gratuita"

Área de atuação assumida no site: de Grândola até Lisboa, passando pelo Alentejo Litoral (Comporta, Melides, Alcácer do Sal), pela Península de Setúbal e pela Grande Lisboa. Confirmar com o cliente se cobre mesmo toda esta faixa.

Enquanto isso não chegar, os botões de telefone e WhatsApp apontam para o formulário em vez de um número inventado.

## Fotografias

Todas as fotografias vêm do [Unsplash](https://unsplash.com), sob a Licença Unsplash: uso comercial permitido, sem pagamento e sem obrigação de atribuição. Não são de domínio público. Foram escolhidas de forma a não mostrarem marcas de outras empresas.
