# Trabalhando com GitHub Flow

**O que é o GITHUB FLOW?**
> O GitHub Flow é um fluxo de trabalho leve, baseado em filiais e grupos, que oferece suporte a equipes e projetos nos quais as implantações são feitas regularmente. 

> Também conhecido como GitHub WorkFlow, o GitHub Flow teve como sua base o Git Flow. Onde foram criadas variações de sua ferramenta como Gitlab Flow, Gitbucket Flow.

**Deseja conhecer mais sobre o Git Flow?** [Clique Aqui](https://github.com/duuh30/gitflow/blob/master/introgitflow.md)

## Começado com GitHub Flow

![Imagem](https://github.com/duuh30/gitflow/blob/master/images/fluxogithubflow.png)

**Falando um Pouco mais sobre o Github Flow**
> No Github Flow seu projeto tem uma branch master singular,onde todo trabalho desenvolvido e liberado vive em todo o processo. Então oque é esse processo e como funciona ? **Vamos Conhecer? Vamos lá !!**



### Criar Branching ou Ramificações
 > Branch ou ramificações é uma parte essencial para o gerenciamento do desenvolvimento paralelo. Onde utiliza-se o Git que é o sistema de controle de versão do Github, que permite criar,destruir e combinar ramificações com o mínino de complexidade. Assim, as ramificações podem existir por quanto tempo você precisar. Quando você cria uma nova ramificação em seu projeto, está criando um ambiente em que você pode experimentar novas ideias, onde suas alterações não afetam sua ramificação Master. Então você está livre para experimentar e confirmar alterações.
 
### Adicionar os commits
 > Depois que você cria uma ramificação, é hora de fazer alterações. Então sempre que você adiciona,edita ou exclui um arquivo, você está fazendo um commit e adicionando. 
 
 **Porque adicionar os Commits?**
 > É essencial para o gerenciamento do novo recurso que esta sendo desenvolvimento, onde a adição desses commits acompanham seu progresso enquanto você trabalha em novos recursos. Além disso, cada commit realizado é considerado uma unidade separada de mudança. Isso permite remover alterações se um Bug crítico for encontrado ou se deseja seguir uma nova alteração de recurso.
 
 ### Abrir um Pedido de Pull Request
 > Oque são esse Pull Request? São um pedido de discussão sobre seus Commits. 
 
 **Mas como assim?**
 > Seus commits eles entram e um estado de périodo probatório,onde suas mudanças estão em analise de aprovação. Para que assim possam revisá-los e discuti-los antes de implantar sua alteração.
 
 **E se não for aprovado?**
 > Se sua alteração não for aprovada, o pedido permanece intacto no Github para futuras referências. Como um registro do processo de tomada de decisão em torno desse conjunto de mudanças.

**E se foi aprovada?**

### Discutir e analisar seu código

> Depois que sua soliticação for aberta, a pessoa ou a equipe que estiver analisando suas alterações poderá realizar perguntas e comentários. Talvez o estilo em que a alteração foi codificada não atende os parametros estabelecidos do projeto, a mudança feita não tenha testes, ou talvez tudo pode ser implementado. 

**Mas e se houver bugs? Se eu esqueci de algo?**
> Se alguém comentar que você esqueceu de faze algo ou se houver um bug no seu código, você pode corrigi-los, e o Github mostrará seus novos commits e qualquer feedback adicional que possa receber na visualização.

### Fase de implantação
> Quando suas alterações passarem pelo processo de análise e discussão, você está com livre acesso para implementar seu código de alteração da ramificação de recursos para a produção, se precisar. 

**Mas e se minha implantação causou problemas?**
> Caso tenha causado problemas, você poderá recupará-la implantando a ramificação Principal existente na produção.

### Fase de Mesclagem

**O que é a fase de mesclagem?**
> É a fase onde suas alterações ja passaram por discussão, revisão de códigos, erros críticos,bugs etc. Então é hora de mesclar seu código a ramificação Principal. 

**Mas se caso eu esqueci o porque dessa mesclagem?**
> O Pull Request guarda um registro das alterações do seu código. Então permite que volte no tempo para entender o porque e como foi a tomada de decisão para a implantação daquela alteração na ramificação Principal.

**Então depois de tudo oque acontece?**
> Então, depois de mesclar a sua antiga ramificação salva as alterações, onde ela pode voltar para entender oque aconteceu. Então a partir dai pode-se deletar essa ramificação feita apenas para a alteração que ja foi implantada na ramificação principal. Ou seja, a ramificação principal junta-se com as alterações. 




**Qual a importância de utilizar o GitHub Flow ?**

> Gerenciar uma mudança pode se tornar um desafio, especialmente para desenvolvimento. É um processo onde muitas pessoas trabalhando em paralelo. O Github Flow atua no controle e sequência de eventos para garantir que cada pessoa utilize a melhor ferramenta no momento certo.Na verdade o GitHub Flow é o gerenciamento de mudanças de processos e pessoas, otimizando para aumentar a produtividade da equipe. O GitHub Flow oferece a flexibilidade para tomar uma decisão de trabalho,onde tudo que é desenvolvido e implementado em sua Branch Master( o Centro do seu Desenvolvimento),onde ele oferece ferramentas de fácil utilização para gerenciar mudanças do seu projeto. 



