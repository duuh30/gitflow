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

