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

**Agora que ja sabemos o que é, e o que são cada branch vamos ao Tutorial**


### Tutorial básico de git flow

**Primeiro, precisamos ter o Git Flow instalado na máquina. Como se trata de uma extensão ao Git, ele não vem instalado com o Git por padrão e para isso precisamos instalá-lo manualmente em sua máquina** **E para provar que não sou cruel😇 , vamos aprender a instalação agora !**

 

**Instalação**

**Ubuntu/Debian-based**
```bash
sudo apt-get install git-flow
```


**Mac OS X**
```bash
brew install git-flow-avh
```


**Windows**
*(Cygwin)*
```bash
wget -q -O - --no-check-certificate https://raw.github.com/petervanderdoes/gitflow-avh/develop/contrib/gitflow-installer.sh install stable | bash
```
*Ou*
```bash
https://git-for-windows.github.io/
```

**Caso tenha mais alguma dúvida existe um Manual de instruções, que pode ser acessado**
```bash
wget --no-check-certificate -q  https://raw.github.com/petervanderdoes/gitflow-avh/develop/contrib/gitflow-installer.sh && bash gitflow-installer.sh install stable; rm gitflow-installer.sh
```



## Com o GitFlow instalado em sua máquina, agora vamos aprender a como trabalhar com o Git Flow 

**Inicialização**
Vamos iniciar o Git Flow com a seguinte instrução
```bash
git flow init
```

**Agora com a inicialização feita, que tal criar uma Nova Feature?**
```bash
git flow feature start NOME_DA_FEATURE
```
> **Lembrando** ao criar uma nova Feature ela começa no seu Branch Atual.

**Agora com sua nova feature feita, vamos publicar no Git?**
Sei que você esta ansioso para ver a mágica acontecer, então use a seguinte instrução!
```bash
git flow feature publish NOME_DA_FEATURE
```

**Que tal obter uma nova Funcionalidade? Um Pull**
> Sei que você esta se perguntando o que danados são um **PULL**.
Então um pull é um mecanismo onde cada desenvolvedor pode gerar uma notificação de conclusão de uma feature qualquer. Isso permite que todos os envolvidos saibam oque esta se passando.

Então utilizamos a seguinte instrução!
```bash
git flow feature pull NOME_DA_FEATURE
```
**E agora vamos finalizar a funcionalidade, pois não se saiu como esperado :(**

Para finalizar a feature feita com tanto carinho, use a instrução abaixo !
```bash
git flow feature finish NOME_DA_FEATURE
```

## Agora vamos trabalhar com as novas versões as Releases 
Você acha que vai ter mais uma dor de cabeça decorando instruções? Nãooooo !
São as mesmas intruções so muda em qual determinada Branch você esta. Vamos lá

**Começar uma nova versão**
```bash
git flow release start NOME_DA_VERSAO
```
> **Lembrando** a nova versão é criada baseado na branch Developer.

**Agora você esta feliz, a versão foi corrigida não existe erros e bugs !** **Vamos Publicar**
**Publicando a versão**
```bash
git flow release publish NOME_DA_VERSAO
```

**Caso precise finalizar a versão**
```bash
git flow release finish NOME_DA_VERSAO
```
> **Lembrando** em toda finalização em qualquer branch que esteja, ela corta todos os vínculos.


## Vamos Trabalhar com a Branch HotFix 
Os Hotfix são feitos para agir imediatamente sobre determinada situação que cause situações indesejadas na versão de aplicação em execução.

**Vamos criar um HotFix**
```bash
git flow hotfix start NOME_DO_HOTFIX
```

> Após a criação de um hotfix, e criado baseado na branch master
> O nome do hotfix e a marcação da versão que apresentou defeitos na execução.

**Finalizando um HotFix**
```bash
git flow hotfix finish MEU_HOTFIX
```

# Qual a importância de utilizar o Github Flow?


