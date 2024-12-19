# Cap 1: React Foundations: About React and Next.js | Next.js
[https://nextjs.org/learn/react-foundations/what-is-react-and-nextjs](https://nextjs.org/learn/react-foundations/what-is-react-and-nextjs)

## O que compoem uma web application?
__Existem alguns componentes que devem ser considerados quando construimos aplicações modernas para web:__
* User Interface (Interface do Usuário): como os usuários irão consumir e interagir com sua aplicação.
* Routing (Roteamento): como os usuários irão navegar entre diferentes partes da sua aplicação.
* Data Fetching (Obtenção de Dados): onde seus dados são armazenados e como você obtêm eles.
* Rendering (Renderização): quando e onde você cria/renderiza seu conteúdo estático ou dinâmico.
* Integrations (Integrações): quais serviços de terceiros você usa (autenticação, pagamentos, CRM), e como você se conecta à eles.
* Infrastructure (Infraestrutura): onde você entrega, armazena e executa o código da sua aplicação (serverless, CDN, edge).
* Performance: como você otimiza sua aplicação para os usuários finais.
* Scalability (Escalabilidade): como sua aplicação se adapta ao seu time, dados e crescimento de tráfego.
* Developer Experience (DevEx): como seu time vive/experiencia a criação e manutenção da sua aplicação.

Para cada ponto definido acima precisamos decidir se iremos criar uma solução própria ou usar ferramentas de terceiros, como pacotes, libs ou frameworks.

**React é uma biblioteca em Javascript para criação de interfaces de usuários interativas**

**Next.js é um framework React que disponibiliza componentes prontos para você criar web applications**

# Cap 2: Rendering User Interfaces (UI)

HTML > DOM > UI
Static > Dynamic > 

# Cap 3: Updating UI with Javascript

```
<html>
    <body>
        <div id="app"></div>
        <script type="text/javascript">
            // Select the div element with 'app' id
            const app = document.getElementById('app');

            // Create a new H1 element
            const header = document.createElement('h1');

            // Create a new text node for the H1 element
            const text = 'Develop. Preview. Ship 🚀';
            const headerContent = document.createTextNode(text);

            // Append the text to the H1 element
            header.appendChild(headerContent);

            // Place the H1 element inside the div
            app.appendChild(header);

        </script>
    </body>
</html>
```

## Programação Imperativa vs. Declarativa
O código acima é um ótimo exemplo de __programação imperativa__. Você está escrevendo os passos para definir como a interface de usuário deve ser atualizada.
Mas quando se trata de criar interfaces de usuários, uma abordagem __declarativa__ é preferida porque isso aumenta a velocidade de desenvolvimento.
Em outras palavras a __programação imperativa__ é como dar instruções passo-a-passo para um chef fazer uma pizza. __Programação Declarativa__ é como pedir uma pizza sem ter conhecimento dos passo necessários para fazer uma pizza. 🍕

# Cap 4: Getting Started with React

## Declarative React Code:
```
<script type="text/jsx">
  const domNode = document.getElementById("app")
  const root = ReactDOM.createRoot(domNode);
  root.render(<h1>Develop. Preview. Ship.</h1>);
</script>
```

## Imperative Javascript Code:
```
<script type="text/javascript">
  const app = document.getElementById('app');
  const header = document.createElement('h1');
  const text = 'Develop. Preview. Ship.';
  const headerContent = document.createTextNode(text);
  header.appendChild(headerContent);
  app.appendChild(header);
</script>
```