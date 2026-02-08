---
description: Workflow para um Agente de IA que lê componentes no Figma via MCP e gera HTML e CSS consistentes com o design system, usando apenas variáveis existentes, seguindo padrões estruturais, garantindo acessibilidade e entregando código documentado.
---

# Workflow do Agente de IA – Criação de Componentes (HTML + CSS)

## Entrada do processo

- Receber o link da **seleção do componente no Figma**
- Validar se o link aponta para um componente ou conjunto de variantes

## Leitura do Figma

- Acessar o arquivo via **Figma MCP**
- Ler a hierarquia de camadas e Auto Layout
- Identificar variantes, estados e propriedades
- Mapear estilos aplicados (cores, tipografia, espaçamentos, bordas)

## Mapeamento de design tokens

- Identificar quais **variáveis já existentes** são usadas no componente
- Relacionar estilos do Figma com os tokens disponíveis
- Não criar novas variáveis em nenhuma hipótese

## Estruturação do HTML

- Seguir o padrão estrutural dos outros componentes do projeto
- Utilizar tags semânticas adequadas
- Manter consistência de classes, wrappers e hierarquia
- Garantir estrutura compatível com variações e estados

## Acessibilidade

- Garantir semântica correta do HTML
- Assegurar navegação por teclado
- Implementar estados de foco visíveis
- Utilizar atributos ARIA apenas quando necessário

## Criação do CSS

- Escrever os estilos exclusivamente no arquivo `components.css`
- Utilizar somente variáveis existentes
- Isolar estilos ao escopo do componente
- Implementar estados como hover, focus, disabled e variações visuais
- Respeitar o cascade e padrões já definidos

## Validação final

- Verificar consistência com outros componentes
- Validar uso correto de tokens e variáveis
- Checar semântica e acessibilidade básica
- Garantir que não houve criação de novos padrões ou variáveis

## Entrega

- Entregar o CSS no arquivo `components.css`
- Fornecer um resumo do que foi feito e das decisões tomadas

---

## Checklist do Agente de IA

- [ ] Acessar o componente via link do Figma MCP
- [ ] Analisar hierarquia, estilos e variantes
- [ ] Mapear e usar apenas tokens existentes
- [ ] Criar HTML seguindo padrões do projeto
- [ ] Garantir acessibilidade básica
- [ ] Escrever CSS somente em `components.css`
- [ ] Implementar estados visuais relevantes
- [ ] Manter consistência com o design system
- [ ] Não criar novas variáveis
- [ ] Entregar resumo do trabalho realizado
