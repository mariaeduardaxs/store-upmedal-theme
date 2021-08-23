# Store Upmedal

The Store Upmedal is based on the basic store front model from VTEX IO Store Framework and the real store https://www.upmedal.com/.

## Configuration

### Step 1 -  Basic setup

Access the VTEX IO [basic setup guide](https://vtex.io/docs/getting-started/build-stores-with-store-framework/1) and follow all the given steps. 

By the end of the setup, you should have the VTEX command line interface (Toolbelt) installed along with a developer workspace you can work in.

### Step 2 - Cloning Store Upmedal

[Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) this repository to your local files to be able to effectively start working on it.

Then, access the repository's directory using your terminal. 

### Step 3 - Editing the `Manifest.json`

Once in the repository directory, it is time to edit the Store Upmedal `manifest.json` file. 

Once you are in the file, you must replace the `vendor` and `account` values. `vendor` is the account name you are working on and `account` is anything you want to name your theme. For example:

```json
{
  "vendor": "storecomponents",
  "name": "my-test-store",
}
```

### Step 4 -  Installing required apps

In order to use Store Framework and work on your store theme, it is needed to have both `vtex.store-sitemap` and `vtex.store` installed.

Run  `vtex list`  and check whether those apps are already installed. 

If they aren't, run the following command to install them: `vtex install vtex.store-sitemap vtex.store -f`

### Step 5 -  Uninstalling any existing theme

By running `vtex list`,  you can verify if any theme is installed.

It is common to already have a `vtex.store-theme`  installed when you start the store's front development process. 

Therefore, if you find it in the app's list, copy its name and use it together with the command `vtex uninstall`. For example:

```json
vtex uninstall vtex.store-theme
```

### Step 6- Run and preview your store

Then time has come to upload all the changes you made in your local files to the platform. For that, use the `vtex link` command. 

If the process runs without any errors, the following message will be displayed: `App linked successfully`. Then, run the `vtex browse` command to open a browser window having your linked store in it.

This will enable you to see the applied changes in real time, through the account and workspace in which you are working. 

If everything looks good, you can create a pull request to colaborate with Store Upmedal!

### Tasks

1. O que precisa cumprir para esse desafio:
    - [x]  Flex layout para ciar cores em CSS
    - [x]  Slider layout para mostrar produtos em destaque 
    - [x]  Criar componente Tab layout para separar produtos por categoria
    - [x]  Criar filtro para puxar a lista de produtos por categoria
    - [x]  Criar um bloco de lista de produto (8 itens por categoria)
    - [x]  Criar e estilizar Minicart para lista dos produtos no carrinho
    - [x]  Ao clicar no produto ir para a tela com Product Summary
    - [x]  Estilizar página de produto
    - [x]  Layout mobile
    - [x]  Criar um componente customizado para falar com suporte no whatsapp no footer
    - [x]  Estilizar footer
    - [x]  Criar um componente customizado para cadastrar leads (possíveis clientes prospectos) - Utilizando components com React
  
            Campos Necessários:
              ○ Nome
              ○ Email
              ○ Telefone
              
      Componente em: [cadastroscomponent](https://github.com/mariaeduardaxs/cadastroscomponent)
    - [ ] Trazer o conteúdo das leads cadastradas no back-end com a API Gateway AWS
    - [ ] Opcional - Criar um item no admin da vtex para trazer o conteúdo das leads cadastradas na API Gateway AWS
