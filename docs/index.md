# Bem-vindo a Documentação do Site de alimentos!

## Visão Geral

Este documento descreve como implementar o protótipo do site de alimentos, que exibe informações nutricionais e históricas de pratos culinários.

## Design

Uma barra de pesquisa para "Valor" (ex.: calorias ou outro filtro nutricional).
Menus dropdown cinzas que expandem para mostrar detalhes do alimento, como nome, origem, valores nutricionais (energia, carboidratos, proteínas, gorduras, sódio) e histórico.
Um cabeçalho visual com imagens de alimentos frescos (frutas, vegetais).

O site é responsivo, com um layout simples e clean, usando tons de verde (para o tema saudável) e cinza/bege para os elementos interativos. Assumimos uma stack web básica: HTML5, CSS3 e JavaScript vanilla (sem frameworks para simplicidade). Para dados, use um array JSON local.
Objetivos funcionais:

Permitir busca por alimentos via barra de pesquisa.
Exibir cards expansíveis (dropdowns) com informações detalhadas.
Tornar o site interativo: expandir/colapsar menus, filtrar resultados.

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
                header-bg.jpg   # Imagem do cabeçalho (frutas/vegetais).
            icons/
                dropdown-icon.svg   # Ícone para dropdown


