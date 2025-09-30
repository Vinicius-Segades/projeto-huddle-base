# Frontend Mentor - Solução da landing page Huddle

Esta é uma solução para o desafio [Huddle landing page with single introductory section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/huddle-landing-page-with-a-single-introductory-section-B_2Wvxgi0). Os desafios do Frontend Mentor ajudam a aprimorar as habilidades de codificação através da construção de projetos realistas.

## Visão Geral

### O Desafio

Os usuários devem ser capazes de:

  - Visualizar o layout ideal para a página, dependendo do tamanho da tela do dispositivo.
  - Ver os estados de *hover* para todos os elementos interativos na página.

### Links

  - URL do Site: (https://vinicius-segades.github.io/projeto-huddle-base/)

## Meu Processo

### Construído com

  - Marcação HTML5 semântica
  - Propriedades customizadas do CSS (variáveis)
  - CSS Grid para o layout principal da página
  - Flexbox para o alinhamento de componentes internos
  - Fluxo de trabalho Desktop-First (responsividade com `max-width`)
  - Font Awesome para os ícones de redes sociais

### O que eu aprendi

Este projeto foi um excelente exercício para solidificar conceitos de layouts responsivos. A principal jornada de aprendizado foi a exploração de diferentes abordagens para a estrutura da página e o posicionamento do plano de fundo.

Inicialmente, utilizamos Flexbox para o layout geral, mas depois migramos para CSS Grid para um controle mais explícito das áreas (`header`, `main`, `footer`). O maior desafio foi garantir que a imagem de fundo única se comportasse corretamente. Através de um processo iterativo, chegamos à solução ideal:

  - **Estrutura com CSS Grid:** Define as áreas principais da página de forma clara.
  - **Plano de Fundo no `body`:** Garante que a imagem de fundo seja contínua e cubra a página inteira sem quebras ou repetições indesejadas.
  - **Abordagem Desktop-First:** Construímos o layout primariamente para telas de desktop e, em seguida, aplicamos uma `media query` com `max-width` para adaptar os estilos a dispositivos menores, garantindo uma boa experiência móvel.

<!-- end list -->

```css
/* Exemplo da abordagem Desktop-First para o background */
body {
    /* O fundo de desktop é definido como padrão */
    background-image: url('../images/bg-desktop.svg');
}

@media (max-width: 768px) {
    body {
        /* Em telas menores, o fundo de mobile sobrescreve o padrão */
        background-image: url('../images/bg-mobile.svg');
    }
}
```

### Desenvolvimento contínuo

Para projetos futuros, pretendo focar em:

  - Adicionar micro-interações e animações com CSS para uma experiência de usuário mais fluida.
  - Explorar o uso de JavaScript para funcionalidades como validação de formulários (caso o botão "Register" se torne um formulário real).
  - Aprofundar em técnicas de otimização de performance, como o carregamento otimizado de imagens e fontes.

## Autor

  - Website - [Vinícius Segades da Silva](https://github.com/Vinicius-Segades)
  - Frontend Mentor - [@Vinicius-Segades](https://www.frontendmentor.io/profile/Vinicius-Segades)
