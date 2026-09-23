## Integração Hyper + Git Bash
Instalação do **Git for Windows**, habilitando comandos no terminal **Hyper**.

 * [Git for Windows](https://gitforwindows.org/)
 * [Hyper](https://hyper.is/)

Na instalação do Git, na tela **Configuring the terminal emulator to use with Git Bash**, selecione a opção **Use Windows' default console window**. As demais opções podem ficar como estão.

Após a instalação do Git e do Hyper, vamos integrar o Hyper com o Git Bash: execute o Hyper, acesse o *menu superior esquerdo > Edit > Preferences*, altere as linhas `fontSize: 12,`, `shell: '',`, `shellArgs: ['--login'],` e `env: {},`, respectivamente, para:

```text
fontSize: 18,
shell: 'C:\\Program Files\\Git\\git-cmd.exe',
shellArgs: ['--command=usr/bin/bash.exe', '-l', '-i'],
env: { 'TERM':'cygwin' },
```

Após configurar, salve, feche e abra o Hyper novamente. As configurações do Hyper serão visualizadas, apresentando o Git Bash integrado.

Instale o plugin `hyper i hyperpower`, feche e abra o Hyper para concluir a instalação. Este plugin faz com que seja exibido um efeito no cursor ao digitar os comandos.

<img width="507" height="134" alt="image" src="https://github.com/user-attachments/assets/0abebf49-224c-4f98-8ab1-e9acdcd28c62" />
