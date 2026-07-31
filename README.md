# bootcamp-aws
Projeto final do Bootcamp AWS usando Amazon Bedrock

## Qual o conteúdo do projeto?
Ele apresenta tanto uma criação e a orquestração de um assistente virtual de delivery para fazer sugestões gastronômicas quanto o planejamento de experiências utilizando o AWS Step Functions.

Para gerenciar esse fluxo de trabalho foi utilizado o Amazon Bedrock para invocar o modelo Claude 3 Haiku, modelo de inteligência artificial generativa.

## Principais Aprendizados

### 1. Orquestração Serverless com AWS Step Function
- Gerenciamento de Estado: aprendi como estruturar fluxos tanto lineares quanto ramificados usando a linguagem ASL (Amazon States Language) para coordenar serviços sem precisar escrever código de infraestrutura complexo. 

- Encadeamento de Prompts: Foi utilizado a saída de um estado anterior para enriquecer e contextualizar a chamada do prompt seguinte, para simular um pensamento estruturado de IA.

### 2. Integração com Amazo Bedrock
- Modelos de Fundação: foi feita a prática com a invocação direta do Claude 3 Haiku (Anthropic) para a geração de texto tanto rápida quanto de baixo custo.

## Tecnologias Utilizadas 
- AWS Step Functions (Orquestrar os Fluxos)
- Amazon Bedrock (Modelos Claude 3 Haiku)
- AWS IAM (Políticas de Segurança e Controle de Acesso)

## Como Executar esse Projeto
1. Solicite o acesso ao modelo desejado na aba `Model Catalog` do Amazon Bedrock na AWS.
2. Crie uma máquina de estados no AWS Step Functions.
3. Selecione o modo de edição em código (JSON) e cole na mesma aba o conteúdo desse repositório.
4. Clique em `Iniciar Execução` (no caso, não é necessária passar dados de entrada, porque os prompts já estão no corpo das etapas).
5. Inspecione o resultado final no histórico de eventos de execução.