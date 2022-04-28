## Git for Windows e Hyper
Instalação do Git for Windows, habilitando comandos no terminal Hyper.

-----------------------------------------

 - [Git for Windows](https://gitforwindows.org/) e [Hyper](https://hyper.is/): Após a instalação de ambos, vamos integrar o Hyper com o Git Bash:
    - execute o Hyper, acesse o *menu superior esquerdo > Edit > Preferences*, altere as linhas `fontSize: 12,`, `shell: '',`, `shellArgs: ['--login'],` e `env: {},`, respectivamente, para:

      ```
      fontSize: 18,
      shell: 'C:\\Program Files\\Git\\git-cmd.exe',
      shellArgs: ['--command=usr/bin/bash.exe', '-l', '-i'],
      env: { 'TERM':'cygwin' },
      ```

    - Após configurar, salve, feche e abra o Hyper novamente. As configurações do Hyper serão visualizadas, apresentando o Git Bash integrado. Para acessar o C:/, diferentemente do cmder, informamos `cd /c/`.
    - Instale o plugin `hyper i hyperpower`, feche e abra o Hyper para concluir a instalação do plugin. Este plugin instala um efeito que exibe um efeito ao digitar os comandos.
