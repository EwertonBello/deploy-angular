# Deploy Angular
Fazendo deploy de um app default do Angular no GitHub Pages<br/>
<Strong>Angular: </Strong>(https://angular.io/)<br/>
<Strong>angular-cli-ghpages: </Strong>(https://www.npmjs.com/package/angular-cli-ghpages)<br/>
<Strong>Demo: </Strong>(https://ewertonbello.github.io/deploy-angular/)

### Procedimento

1. Crie um repositório e vincule seu projeto a ele, na pasta do seu projeto faça:
    ```
    git init
    git add .
    git commit -m "primeiro commit"
    git remote add origin https://github.com/NomeDeUsuario/nome-do-repositorio.git
    git push -u origin master
    ```
2. Depois faça o build do seu projeto, `ng build --prod --base-href "https://USERNAME.github.io/REPOSITORY_NAME/"`.<br/>
Exemplo:`ng build --prod --base-href "https://ewertonbello.github.io/deploy-angular/"`

3. Depois utilize o comando `npx angular-cli-ghpages --dir=dist/[PROJECTNAME]` para fazer o deploy da pasta de produção do seu app no branch gh-pages, utilizando o pacote angular-cli-ghpages.<br/>
Exemplo: `npx angular-cli-ghpages --dir=dist/deploy-angular`
