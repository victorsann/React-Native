<div align="center">
 <img src="./assets/react.png">
</div>

Existem duas pricipais formas de desenvolver uma aplicação em React Native atualmente. Elas são:

<h1>React Native</h1>

Iniciar um projeto utilizando a React Native CLI é recomendado quando houver a necessidade contato com código nativo, o que implica em certas "obrigações" em termos de desenvolvimento. Tal meio permite permite criar uma aplicação completa, incuindo as pastas android e ios, além de acomanhar o Typescript:

    npx react-native init <project-name>

Como resultado será criada a seguite estrutura de diretórios e arquivos:

> project-name
> |
> ├── _test_
> ├── .bundle -----------------
> ├── android -----------------
> ├── ios
> ├── node_modules
> ├── .eslintcr.js
> ├── .gitignore
> ├── .prettierrc.js
> ├── .watchmanconfig
> ├── app.json
> ├── App.tsx
> ├── babel.config.js
> ├── Gamfile
> ├── index.js
> ├── jest.config.js
> ├── metro.config.js
> ├── package-lock.json
> ├── package.json
> ├── README.md
> ├── tsconfig.json
> |\_\_ yarn.lock

<h1>Expo GO</h1>

Expo allows you to create three different types of project structure:

<h2>1. Managed workflow:</h2>

    npx create-expo-app --template

Como resultado será criada a seguite estrutura de diretórios e arquivos:

    project-name
    |
    ├── assets
    ├── node_modules
    ├── .gitignore
    ├── App.js
    ├── app.json
    ├── babel.config.js
    ├── package-lock.json
    |__ package.json

<h2>2. Bare workflow:</h2>

O Bare Workflow fornece controle completo sobre o código nativo, permitindo que os desenvolvedores adicionem qualquer módulo nativo ou modifiquem os existentes. Esta flexibilidade é crucial para projetos complexos com requisitos específicos. Sua estrutura parte da conversão do managed workflow a partir do seguinte comando:

    npx expo prebuild

Como resultado será criada a seguite estrutura de diretórios e arquivos:

    project-name
    |
    ├── .expo
    ├── android
    ├── ios
    ├── assets
    ├── node_modules
    ├── .gitignore
    ├── App.js
    ├── app.json
    ├── babel.config.js
    ├── package-lock.json
    |__ package.json

<h2>Migração: Do Expo para React Native</h2>

<h2>3. Development Builds</h2>
