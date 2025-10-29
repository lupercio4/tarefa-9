# 🌿 Projeto Recycle

O **Recycle** é um site informativo e interativo desenvolvido para promover a reciclagem e apresentar o funcionamento de uma máquina acadêmica que transforma o descarte correto de PETs e latas em uma experiência moderna e recompensadora.

---

## 📁 Estrutura do Projeto

```
📂 tarefa-9/
├── index.html
├── css/
│   ├── reset.css
│   └── style.css
├── js/
│   └── script.js
└── img/
    ├── pasta com diversas imagens ilustrativas
```

Todo o conteúdo do site está centralizado em um único arquivo **index.html**, acompanhado de arquivos externos de estilo e script.

---

## 🌍 Tema do Site

O projeto une **sustentabilidade e tecnologia**, incentivando a consciência ambiental nas instituições de ensino.  
A máquina Recycle simboliza a inovação verde — transformando o lixo reciclável em recompensas.

O site apresenta:
- O funcionamento da máquina;
- Benefícios da reciclagem;
- Depoimentos de usuários;
- Curiosidades e estatísticas sobre impacto ambiental.

---

## 🧱 Tecnologias Utilizadas

| Tecnologia | Função |
|-------------|--------|
| **HTML5** | Estrutura e organização das seções |
| **CSS3** | Layout, responsividade e design temático |
| **JavaScript (ES6)** | Interatividade, animações e lógica de eventos |
| **Vercel** | Deploy e hospedagem do site |
| **Git / GitHub** | Versionamento e publicação do código |

---

## 📜 Estrutura do Código

### 🟢 index.html
Reúne todas as seções do site:
- Cabeçalho fixo com menu e login;
- Seção Hero com destaque visual;
- Cards explicando o uso da máquina;
- Vídeo demonstrativo do projeto;
- Contadores animados de reciclagem;
- Linha do tempo da história da reciclagem;
- Política de uso e parcerias;
- Curiosidades e especificações técnicas;
- Botões flutuantes (modo escuro e topo).

### 🟡 style.css
Mais de **400 linhas**, com:
- Design responsivo via *flexbox*;
- Paleta de cores naturais;
- Modo escuro completo;
- Efeitos hover e transições suaves;
- Animações de entrada (`.revelado`);
- Estilização de tabelas, cards e rodapé.

### 🟣 reset.css
Remove estilos padrões dos navegadores.

### 🔵 script.js
Mais de **300 linhas** e **10 eventos JavaScript** implementados:

1. **Efeito Hover** — troca de ícones e cores dos cards.  
2. **Modo Escuro/Claro** — alterna tema com botão e tecla “T”.  
3. **Botão “Voltar ao Topo”** — rolagem suave até o início.  
4. **Efeito Typewriter** — texto animado no título principal.  
5. **Scroll Suave** — transição leve ao clicar em links âncora.  
6. **Header Dinâmico** — o menu some no scroll e reaparece.  
7. **Animações ao Rolar** — exibe seções com IntersectionObserver.  
8. **Menu Hambúrguer** — alterna visibilidade no mobile.  
9. **Contadores Animados** — incrementam valores em tempo real.  
10. **Atalhos de Teclado** — alternância de tema e controle de foco.

---

## 💡 Explicação dos Eventos JavaScript

Cada evento foi programado com foco em experiência do usuário e clareza no código.

### 🔸 Hover em Cards
Detecta `mouseenter` e `mouseleave` para trocar imagens e cores dinamicamente.
```js
card.addEventListener("mouseenter", () => {
  img.src = hoverSrc;
  card.style.color = "#6d8140";
});
```

### 🔸 Tema Claro/Escuro
Usa `localStorage` para lembrar o tema escolhido pelo usuário.
```js
function ativarModoEscuro() {
  document.body.classList.add('tema-escuro');
  localStorage.setItem('temaRecycle', 'escuro');
}
```

### 🔸 Rolagem Suave
Implementada com `scrollIntoView()` para transições leves entre seções.

### 🔸 Header Dinâmico
Detecta movimento de rolagem e esconde o cabeçalho automaticamente, liberando mais espaço visual.

### 🔸 Contadores
Usam incremento gradual para dar a sensação de progressão animada:
```js
const increment = target / 200;
if (count < target) counter.innerText = count + increment;
```

Essas funções garantem um site **interativo e otimizado**, sem sobrecarregar o navegador.

---

## 🧩 Responsividade

O site foi desenvolvido com *media queries* para telas menores (até 600px), ajustando:
- Layout da seção Hero (coluna reversa);
- Ocultação dos botões flutuantes;
- Redução de fontes e espaçamentos;
- Menu móvel tipo hambúrguer.  

Isso garante boa visualização tanto em **celulares** quanto em **computadores**.

---

## 🌗 Design do Modo Escuro

O modo escuro modifica toda a paleta visual com tons cinza e verde-oliva.  
As cores se invertem mantendo contraste ideal para leitura.

Principais mudanças:
- Fundo escurecido (`#121212`);
- Bordas verdes (`#6d8140`);
- Cards e tabelas redesenhados com `box-shadow` leve;
- Botões gradientes alterados via `linear-gradient()`.

---

## 🧠 Estrutura Lógica do JavaScript

O código é dividido em blocos lógicos:
1. **Inicialização geral (`DOMContentLoaded`)**
2. **Funções auxiliares (scroll, tema, animações)**
3. **Eventos principais (hover, click, keydown)**
4. **Animações automáticas (observer, contador)**

Essa separação facilita a manutenção e legibilidade.

---

## 🧩 Melhorias Futuras

- Adicionar sistema real de login e pontuação via backend.  
- Integrar API para contabilizar materiais reciclados.  
- Inserir dashboard com estatísticas por usuário.  
- Aplicar Progressive Web App (PWA) para uso offline.  

Essas ideias ampliariam a funcionalidade e a aplicação prática do projeto.

---

## ⚙️ Requisitos Atendidos

- [x] HTML com mais de 700 linhas  
- [x] CSS com mais de 400 linhas  
- [x] JS com mais de 300 linhas  
- [x] README.md com mais de 200 linhas  
- [x] 5+ eventos JavaScript funcionais  
- [x] Publicação no GitHub e Vercel  
- [x] Códigos comentados  
- [x] Design responsivo e modo escuro

---

## 🌐 Links do Projeto

- GitHub: [https://github.com/lupercio4/tarefa-9](https://github.com/lupercio4/tarefa-9)
- Vercel: [https://tarefa-9-gamma.vercel.app/](https://tarefa-9-gamma.vercel.app/)

---

## 🧩 Autor

**Nome:** Lupercio Neto  
**Curso:** Engenharia da Computação – FACENS  
**Tema:** Sustentabilidade e Inovação Tecnológica  
**Objetivo:** Criar um site funcional e educativo sobre reciclagem.

---

## 📘 Conclusão

O **Recycle** combina interatividade e propósito ambiental.  
Seu desenvolvimento aplicou todos os fundamentos de **HTML, CSS e JavaScript**, resultando em um site completo, moderno e educativo.  
Cada linha do código foi comentada para facilitar a compreensão técnica e a manutenção futura.

> 🌱 “Reciclar é transformar o presente para preservar o futuro.”