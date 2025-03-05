# Software that we will use. 

1. VSCode
El programa Visual Studio Code (VSCode) es una integrated development environment (IDE), es decir un programa que permite interpetar y programar en diversos lenguajes, es como un motor de programacion. Para descargarla, accede a la [web de VSCode](https://code.visualstudio.com/Download).

Una vez dentro, selecciona tu sistema operativo: macOS, Windows, Linux. Descarga la version mas reciente. 

3. Python
Todo este curso se va a desarrollar en python. El motivo, es gratis, y es el lenguaje de programacion mas usado en el mundo, pero sobre todo por que es gratis. Para ello debeis ir a la [web](https://www.python.org/downloads/) y descargaros la version (check version) para vuestro sistema operativo. 

4. Setup de la terminal (copy the one from tryg)




6. Setup de las extensiones (copy the ones from tryg)
7. Crear un virtual environment.


Una vez instalado el source vamos a pegar estas linias en el .zshsrc . Esto permite que tan solo escribiendo 'activate' y 'deactivate' en una carpeta que contenga un virtual environment, dicha orden se ejecute automaticamente.

Ademas aniade dos alias, c para clear, y ll para ls -la, que va a permitir inspeccionar todos los archivos y directorios de una carpeta cualquiera. 
```bash
alias ll="ls -la"
alias c="clear"


if [[ $(which virtualenvwrapper.sh) != "virtualenvwrapper.sh not found" ]]; then
  export PROJECT_HOME=$HOME/projects
  export WORKON_HOME=$HOME/.virtualenvs
  export VIRTUALENVWRAPPER_PYTHON=$(which python3)
  source virtualenvwrapper.sh
fi

if [[ $(which helm) != "helm not found" ]]; then
  source <(helm completion zsh)
fi

if [[ $(which chef) != "chef not found" ]]; then
  source <(chef shell-init zsh)
fi

# Function to simplify virtual environment activation
function activate() {

    # Check for activated environment
    if test -v VIRTUAL_ENV
    then
      CURRENT_ENV=${VIRTUAL_ENV%/*}

      if test "${PWD}" = "${CURRENT_ENV}"
      then
        print -P "$fg[green]Environment is already active."
        return 0
      elif test -n "${VIRTUAL_ENV}"
      then
        print -P "$FG[208]Deactivating existing environment."
        deactivate
      fi
    fi

    if [[ -d .venv ]]
    then
        source .venv/bin/activate && print -P "$fg[green]Environment activated." || print -P "$FG[196]Activation failed!"
    else
        print -P "$FG[229]No environment found in '${PWD}/.venv'"
    fi
}
```