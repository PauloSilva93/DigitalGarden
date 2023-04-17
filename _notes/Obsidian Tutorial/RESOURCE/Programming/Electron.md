# Electron

## Início rápido

1. Instale o Node.js versão LTS que pode ser baixado aqui: https://nodejs.org/en/download/
2. Crie uma pasta ElectronApp e abra no VS Code.
3. No terminal do VS Code, execute `npm init -y`. Este comando criará o arquivo package.json com as configurações padrão para o aplicativo.
4. Execute o comando `npm install --save-dev electron`. Este comando criará as dependências necessárias do Electron na pasta `node_modules`.
5. Substitua o corpo do objeto scripts por `"start": "electron ."` para que possamos executar o app pelo comando `npm run start`. O objeto scripts ficará assim:

```js
"scripts": {
	"start": "electron ."
}
```

6. Crie um arquivo index.js na pasta ElectronApp. Ele é o arquivo apontado no package.json como "main". Cole o conteúdo abaixo:

```js
const { app, BrowserWindow } = require('electron')

const createWindow = () => {
    const win = new BrowserWindow({
      width: 800,
      height: 600,
      webPreferences: {
        nodeIntegration: true,
        contextIsolation: false,
      }
    })
  
    win.loadFile('index.html')
  }

  app.whenReady().then(() => {
    createWindow()
  })

  app.on('window-all-closed', () => {
    if (process.platform !== 'darwin') app.quit()
  })
```

7. Crie um arquivo index.html na pasta ElectronApp. Ele é referenciado no arquivo index.js em `win.loadFile('index.html')`. Cole o conteúdo abaixo:

```js
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Electron App</title>

    <h1>ELECTRON APP</h1>

    <button onclick="execCmd()">execute algo...</button>

    <script src="script.js"></script>
</head>
<body>
    
</body>
</html>
```

8. Crie um arquivo script.js que já está referenciado em index.html e cole o conteúdo abaixo:

```js
const { exec } = require("child_process");

function execCmd() {
    exec("start c:", (error, stdout, stderr) => {
        if (error) {
            console.log(`error: ${error.message}`);
            return;
        }
        if (stderr) {
            console.log(`stderr: ${stderr}`);
            return;
        }
        console.log(`stdout: ${stdout}`);
    });
}
```

9. Execute a aplicação no terminal pelo comando `npm start`

10. Para distribuir a aplicação, gerando um .exe, primeiro devemos instalar o módulo `electron-packager` com o comando `npm install electron-packager -g`.
Depois executamos `electron-packager ./ ElectronApp --platform=win32 --arch=x64` para gerar o app com o nome ElectronApp para sistemas x32 no mesmo diretório do projeto.
