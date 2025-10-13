# Bem-vindo a Documentação do Site de alimentos!

## Visão Geral

Este documento descreve como implementar o protótipo do site de alimentos, que exibe informações nutricionais e históricas de pratos culinários.

## Design

Uma barra de pesquisa para "Valor" (ex.: calorias ou outro filtro nutricional).
Menus dropdown cinzas que expandem para mostrar detalhes do alimento, como nome, origem, valores nutricionais (energia, carboidratos, proteínas, gorduras, sódio) e histórico.


O site é responsivo, com um layout simples e clean, usando tons de verde (para o tema saudável) e cinza/bege para os elementos interativos. Assumimos uma stack web básica: HTML5, CSS3 e JavaScript vanilla (sem frameworks para simplicidade). Para dados, foi usado um array JSON local.

Objetivos funcionais:
Permitir busca por alimentos via barra de pesquisa.
Exibir cards expansíveis (dropdowns) com informações detalhadas.
Tornar o site interativo: expandir/colapsar menus, filtrar resultados.

##Passo a Passo: Como Usar o Site!

* Acessando o Site

Abra o navegador (Chrome, Firefox, Safari ou Edge).
Digite o URL do site (ex.: http://localhost:5500/index.html se rodando localmente via Live Server, ou o domínio real quando hospedado).
A página carrega com o header verde no topo, barra de busca abaixo e lista de cards de alimentos.

* Navegando pela Lista de Alimentos

Visualização Inicial: Os cards aparecem como menus cinzas compactos, mostrando apenas o nome do prato (ex.: "Estrogonofe").

Expandir um Card: Clique no cabeçalho cinza do card (o nome do prato).

O card expande suavemente para baixo, revelando:

Imagem do Prato: Foto ilustrativa.
Nome e Região de Origem: Ex.: "Nome: Estrogonofe | Região: Rússia, Europa".
Valores Nutricionais: Lista em grade (duas colunas no desktop, uma no mobile)

História: Parágrafo curto sobre a origem (ex.: explicações sobre a família Stroganov).

Para fechar: Clique novamente no cabeçalho cinza. O ícone de seta (▼) rotaciona para indicar o estado (aberto/fechado).

Rolagem na Lista: Se houver muitos pratos (ex.: 10+), use o mouse wheel, barra lateral ou toque (mobile) para rolar apenas a seção de alimentos. O header e a busca ficam fixos no topo.

* Usando a Barra de Pesquisa

Localização: Logo abaixo do header, um campo branco arredondado com placeholder "Valor (ex: calorias)".
Como Pesquisar:

Digite um termo no campo:

Por Nome: Ex.: "estro" → Filtra para "Estrogonofe".
Por Valor Nutricional: Ex.: "275" → Mostra pratos com energia próxima a isso.
Combinações: Funciona para qualquer parte dos dados (nome, região, nutrientes).


Os resultados atualizam em tempo real (à medida que você digita).
Para limpar: Clique no × ao lado do campo ou apague o texto manualmente.

* Dicas:

Pesquisas são case-insensitive (não diferencia maiúsculas/minúsculas).
Se não houver resultados, a lista fica vazia — tente termos mais gerais.
No mobile, o teclado aparece automaticamente ao tocar no campo.

## Project layout

    mkdocs.yml    # The configuration file.
    site-alimentos/
        index.html  # Página principal.
        styles.css  # Estilos globais.
        script.js   # Lógica interativa.
        data/
            alimentos.json   # Dados dos alimentos (JSON).
        assets/
            images/
                image.jpg   # Imagem dos alimentos.
            icons/
                icon.svg   # Favicon do site.





