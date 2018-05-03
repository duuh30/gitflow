# Trabalhando com Git Flow

**O que é o GIT FLOW?**
> O GitHub Flow é um fluxo de trabalho leve, baseado em filiais e grupos, que oferece suporte a equipes e projetos nos quais as implantações são feitas regularmente. 
> Trata-se de um modelo de organização de branches (ramificações), isto significa que Git Flow estabelece regras e nomenclaturas para cada tipo de Branches, que define o que cada branch e capaz de realizar.

**Vamos conhecer algumas delas?**  **Vamos Lá!**
- Branch Master
> É a branch que contém todo o código da sua aplicação estável.

- Branch Developer  
> É a branch que contém código em nivel de preparação para o próximo deploy. Então todas as features que são finalizadas são juntas com a Branch Developer e testadas, e somente depois a branch developer é preparada para juntar com a branch master. 

**Mas o que é Deploy e Feature?**
> Deploy é o momento em que você lança uma nova versão da sua aplicação e publica ele no seu Servidor.
> Feature são as novidades da sua aplicação, no caso são as novas funcionalidades e versões.

- Branch Features 
> Como dito acima são branches que são desenvolvidas novas funcionalidades para o projeto em execução. Essas branches são criadas a partir da branch develop, e ao final, são juntas a branch Develop.

- Branch Hotfix
> São as branches onde são realizadas todos os tipos de correções de erros críticos encontrado nos projetos em execução. Onde esses tipos de branches são criadas pela **Branch Master**, e logo após as correções são juntas a **Branch Master** e a **Branch Developer**, pois os próximos deploys devem receber as correções dos Bugs.

- Branch Release
> É a branch onde guarda todas as versões da aplicação,nessa branches bugs encontrados durante os testes das features que vão para produção podem ser corrigidos mais tranquilamente, antes de irem efetivamente para produção. 

**Agora que ja sabemos o que é, e o que são cada branch vamos ao** ### Tutorial


