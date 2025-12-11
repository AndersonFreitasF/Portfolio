# Template Portfolio Profissional

Template de portfólio profissional e responsivo, desenvolvido com HTML, Tailwind CSS e JavaScript puro. Design moderno com efeitos de glassmorphism, animações suaves e visual dark mode.

## Características

- **Design Moderno**: Interface dark com tema verde limão personalizável
- **100% Responsivo**: Funciona perfeitamente em desktop, tablet e mobile
- **Performance Otimizada**: Carregamento rápido e animações fluidas
- **Efeitos Visuais**: Glassmorphism, gradientes e microanimações
- **Modal de Projetos**: Galeria de imagens com navegação por teclado
- **Seções Completas**: Home, Sobre, Experiência, Projetos e Contato
- **Marquee de Tecnologias**: Carrossel infinito com seus skills
- **Fácil Customização**: Comentários detalhados em português

## Demonstração ao Vivo

Confira o template funcionando: [Anderson Freitas | Fullstack Developer](https://portfolio-55y6.onrender.com)

## Personalizando as Cores

Para alterar a cor principal (verde limão por padrão), edite o arquivo `Template.html`:

```javascript
// Procure por esta seção no <script> do head:
colors: {
  background: "#09090b",  // Cor de fundo
  surface: "#18181b",     // Cor dos cards
  border: "#27272a",      // Cor das bordas
  primary: "#a3e635",     // Mude esta cor aqui
  secondary: "#ecfccb",   // Cor secundária
}
```

Substitua `#a3e635` pelo código hexadecimal da sua cor preferida.

## Editando o Conteúdo

### 1. Informações Pessoais

Procure e substitua os seguintes textos no HTML:

- **Nome**: `SEU NOME` → Seu nome real
- **Profissão**: `Sua Profissão ou Especialidade` → Sua área de atuação
- **Logo**: `LOGO.` → Suas iniciais ou marca

### 2. Seção Sobre Mim

Edite os três parágrafos na seção "A Jornada":

```html
<p>[Parágrafo 1]: Escreva sobre como você começou.</p>
<p>[Parágrafo 2]: Escreva sobre o que você faz hoje.</p>
<p>[Parágrafo 3]: Escreva sobre seus hobbies ou objetivos futuros.</p>
```

### 3. Experiência Profissional

Para cada experiência, altere:

```html
<h3>Nome do Cargo</h3>
<span>Ano - Presente</span>
<span>Nome da Empresa</span>
<span>Cidade, Estado</span>
<p>Descrição detalhada das atividades...</p>
```

### 4. Configurando Projetos

Os projetos são configurados via **JavaScript**. Procure por estas seções no final do HTML:

#### 4.1 Imagens do Carrossel

```javascript
const projectImages = {
  project1: [
    { url: "link-da-imagem-1.jpg", alt: "Descrição" },
    { url: "link-da-imagem-2.jpg", alt: "Descrição" },
    { url: "link-da-imagem-3.jpg", alt: "Descrição" },
  ]
};
```

#### 4.2 Desafios Técnicos

```javascript
const projectChallenges = {
  project1: [
    "Desafio 1: Descrição",
    "Desafio 2: Descrição",
    "Desafio 3: Descrição",
  ]
};
```

#### 4.3 Aprendizados

```javascript
const projectLearnings = {
  project1: [
    "Aprendizado 1",
    "Aprendizado 2",
    "Aprendizado 3",
  ]
};
```

#### 4.4 Links e Informações

```javascript
const projectInfo = {
  project1: {
    title: "Nome Completo do Projeto",
    repoUrl: "https://github.com/seu-usuario/projeto",
    liveUrl: "https://seu-projeto.com",
    description: "Descrição detalhada do projeto..."
  }
};
```

## Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **Tailwind CSS**: Framework CSS via CDN
- **JavaScript Vanilla**: Interatividade sem frameworks
- **Lucide Icons**: Ícones modernos e leves
- **Devicon**: Ícones de tecnologias
- **Google Fonts**: Tipografia (Inter + Space Grotesk)

## Como Usar

1. **Clone ou baixe** o arquivo `Template.html`
2. **Renomeie** para `index.html`
3. **Edite** o conteúdo conforme as instruções acima
4. **Hospede** em qualquer serviço:
   - GitHub Pages
   - Render
   - Vercel
   - Seu próprio servidor

## Estrutura de Pastas

```
portfolio/
│
├── index.html          # Arquivo principal (Template.html renomeado)
└── README.md           # Este arquivo
```

Não precisa de nenhuma pasta adicional! Tudo está em um único arquivo HTML.

## Deploy Rápido

### GitHub Pages

1. Crie um repositório no GitHub
2. Faça upload do `index.html`
3. Vá em **Settings** → **Pages**
4. Selecione a branch **main** e salve
5. Seu site estará em: `https://seu-usuario.github.io/nome-do-repositorio/`

## Customização Avançada

### Velocidade do Marquee (Carrossel de Tecnologias)

```css
/* Procure por esta animação no <style> */
animation: scroll 40s linear infinite;
/*                 ↑ Mude este valor */
/* 
  - Valores maiores = mais lento
  - Valores menores = mais rápido
*/
```

### Adicionar Mais Tecnologias no Marquee

```html
<!-- Adicione mais ícones dentro do marquee-content -->
<i class="devicon-python-plain colored text-4xl opacity-80 hover:opacity-100 transition-opacity" title="Python"></i>
```

Consulte todos os ícones disponíveis em: [devicon.dev](https://devicon.dev/)

## Funcionalidades Mobile

- Menu hambúrguer responsivo
- Touch-friendly em todos os elementos
- Otimizado para telas pequenas
- Galeria de projetos adaptável

## Solução de Problemas

### Ícones não aparecem?

Verifique se tem conexão com a internet (os ícones vêm de CDN).

### Modal não abre?

Certifique-se de que o `onclick="openProjectModal('project1')"` no HTML corresponde ao ID em `projectImages`.

### Formulário não funciona?

O formulário é apenas uma simulação, assim como os botões de rede social. Para receber emails de verdade, integre com:
- [Formspree](https://formspree.io/)
- [Netlify Forms](https://www.netlify.com/products/forms/)
- Seu próprio backend

## Licença

Este template é de **uso livre**. Você pode modificar, distribuir e usar em projetos pessoais ou comerciais.

## Contribuindo

Sugestões e melhorias são bem-vindas. Sinta-se à vontade para:

- Reportar bugs
- Sugerir novas features
- Fazer fork e criar sua própria versão

## Suporte

Encontrou algum problema ou tem dúvidas? Abra uma issue ou entre em contato.

---

**Desenvolvido para a comunidade dev**
