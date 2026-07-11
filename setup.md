# Criando pasta  

- Crie uma pasta chamada ```PLAYLIST```

# Criando subpasta 

Na sua **IDE** *(VS Code)*, caso esteja utilizando outra IDE não precisa criar essa pasta.

- Crie uma pasta ```.VSCODE```
- Crie outra pasta ```settings.json``` Ele serve para dar instruções ao seu editor de código (o Visual Studio Code) sobre como organizar o seu projeto de Python.

# Excluindo arquivos pré copilados (**Escondendo a "bagunça" (files.exclude)**)

Quando você roda um código Python, o computador cria automaticamente vários arquivos de "bastidores" para fazer o código rodar mais rápido na próxima vez. Como você não precisa ler nem editar esses arquivos, este bloco diz ao editor de código: "Por favor, esconda esses arquivos da minha tela para manter meu projeto limpo."

* ``` "/*.pyc": {"when": "$(basename).py"}: ```Esconde os arquivos com final .pyc (arquivos traduzidos pelo computador), mas apenas quando o arquivo .py original (o código que você escreveu) estiver na mesma pasta.

* ``` "/__pycache__": true:``` Esconde pastas chamadas __pycache__. É lá que o Python guarda aqueles arquivos de bastidores. O true significa "Sim, esconda isso".

* ``` "/*.pyteste__cache": true:```  Esconde arquivos gerados por uma ferramenta chamada "pytest" (usada para testar se o código está funcionando).

Código: 

```

{
    "files.exclude":  {
        "**/*.pyc": {"when": "$(basename).py"},
        "**/__pycache__": true,
        "**/*.pyteste__cache": true    
    },
    "python-envs.defaultEnvManager": "ms-python.python:system",
    "python-envs.defaultPackageManager": "ms-python.python:pip"
}

```

# Terminal Bash 

Agora vamos deixar nosso arquivo pronto para o git.

Código: 

```
git init

```
