# Commits Semânticos

### _Estrutura._
``` 
<tipo>[escopo opcional]: <descrição>
<corpo opcional>
<rodapé opcional>
````
### Tipos 
 + build: Alterações que afetam o sistema de construção ou dependências externas (escopos de exemplo: gulp, broccoli, npm),
+ ci: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs);
+ docs: referem-se a inclusão ou alteração somente de arquivos de documentação;
+ feat: Tratam adições de novas funcionalidades ou de quaisquer outras novas implantações ao código;
+ fix: Essencialmente definem o tratamento de correções de bugs;
+ perf: Uma alteração de código que melhora o desempenho;
+ refactor: Tipo utilizado em quaisquer mudanças que sejam executados no código, porém não alterem a funcionalidade final da tarefa impactada;
+ style: Alterações referentes a formatações na apresentação do código que não afetam o significado do código, como por exemplo: espaço em branco, formatação, ponto e vírgula ausente etc.);
+ test: Adicionando testes ausentes ou corrigindo testes existentes nos processos de testes automatizados (TDD);
+ chore: Atualização de tarefas que não ocasionam alteração no código de produção, mas mudanças de ferramentas, mudanças de configuração e bibliotecas que realmente não entram em produção;
+ env: basicamente utilizado na descrição de modificações ou adições em arquivos de configuração em processos e métodos de integração contínua (CI), como parâmetros em arquivos de configuração de containers.


Também, o Guidelines, recomenda o tipo improvement para commits que melhoram uma implementação atual sem adicionar um novo recurso ou consertar um bug.

Observe que esses tipos não são obrigatórios pela especificação do Conventional Commits.

Reforço que estes são os principais tipos utilizados, mas existem outros diversos que podem ser empregados e também serem adequados a necessidade de sua equipe de desenvolvimento.

Escopos
Um escopo pode ser adicionado ao tipo do commit, sendo um parâmetro opcional, para fornecer informações contextuais adicionais e está contido entre parênteses, por exemplo feat(parser): adiciona capacidade de interpretar arrays.

Normalmente, a utilização do escopo acontece em commits específicos e pontuais, os quais necessitam especificar o contexto imediato da mudança executada pelo commit, como em um módulo de login, middleware ou profile.

Por exemplo, um processo de refactor nas configurações de rotas do módulo de login de seu projeto. Poderíamos descrever, utilizando o escopo, da seguinte forma o nosso commit semântico:

feat(login/routes): change in route settings for the login
Descrições
As descrições se trata de um dos parâmetros obrigatórios da sintaxe, e devem ser preferencialmente apresentadas com letras minúsculas, e obrigatoriamente iniciando com letra minúscula, suportando letras maiúsculas em descrição de arquivos ou classes específicas.

Também devem ser suficientemente claras, utilizando seu espaço até o máximo permitido da linha.

test: ensure DbLoadSurveys throws if LoadSurveysRepository throws
Corpo
O corpo, por sua vez, caracteriza-se por ser opcional e raramente recomendado sua utilização.

Resumindo-se em casos que necessitem de uma apresentação mais completa do conteúdo implantado no commit, o qual a descrição anterior não foi o suficiente para elucidar e esclarecer.

Podendo conter descrições mais precisas do que está contido no commit, apresentando impactos e os motivos pelos quais foram empregadas as alterações no código, como também instruções essenciais para intervenções futuras.

O corpo DEVE iniciar com uma linha em branco após a descrição. Um corpo de confirmação é de forma livre e pode consistir em qualquer número de parágrafos separados por nova linha.

feat: ensure LoadSurveysController returns 204 if there is no content
- Returns code 204 if the search load method does not return content
Rodapé
Por fim o rodapé também não possui uso obrigatório. Restringindo-se às alterações de estado via smart commit, como resoluções de problemas (issues), através de chamados de atendimentos, ou sprints de projetos de implantação os quais podem ser descritos no rodapé.

Pode ser fornecido um ou mais rodapés, o primeiro sempre iniciando uma linha em branco após o corpo. Cada rodapé deve consistir em um token de palavra, seguido pelo símbolo “:” (dois pontos) e posteriormente um espaço em branco e o símbolo “#” (sustenido) como separador da string descritiva do rodapé (conceito inspirado na convenção do Git Trailer).

O token de um rodapé DEVE usar o símbolo “-” (hífen) no lugar de caracteres de espaço em branco, por exemplo, Reviewed-by, permitindo uma diferenciação de um rodapé em relação a um corpo com vários parágrafos.

fix: correct minor typos in code
see the issue for details
on typos fixed.
Reviewed-by: Elisandro Mello
Refs #133
Pronto, agora você já sabe o que precisa sobre commits!

Vale ressaltar que, de forma gradativa, pode-se introduzir e adequar a padronização à cultura de seu time de desenvolvimento, ou mesmo ao seu uso pessoal.

Deixe seus comentários e divulgue caso tenha gostado, pois ajuda esse colega a divulgar seu trabalho.

