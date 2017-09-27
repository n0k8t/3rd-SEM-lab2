## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [X] 1. Ознакомиться со ссылками учебного материала
- [X] 2. Выполнить инструкцию учебного материала
- [X] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial
Устанавливаем значение переменных окружения `GITHUB_USERNAME` и `GIST_TOKEN`
```bash
$ export GITHUB_USERNAME=n0k8t	#Устанавливаем значение переменную окружения `GITHUB_USERNAME`
$ export GIST_TOKEN=xxxxxxxxxxxxxxxxxxxxx #Устанавливаем значение переменную окружения `GIST_TOKEN`
$ alias edit=nano #Переопределяем команду edit
```
Устанавливаем `gistup`
```bash
$ npm install -g gistup #установливаем gistup
```
Добавляем токен в файл gist'a
```bash
$ cat > ~/.gistup.json <<EOF
{
  "token": "${GIST_TOKEN}"
}
EOF #заполняем файл .gistup.json
```
Создаем рабочее пространство 
```bash
$ cd ~	#переход в домашнюю директорию 
$ mkdir -p workspace/labs/projects/	#создаем директроию workspace/labs/projects/
$ mkdir -p workspace/labs/tasks/	#создаем директроию workspace/labs//tasks/
$ mkdir -p workspace/labs/reports/	#создаем директроию workspace/labs/reports/	
```

## Report 
Добавляем `Report` на `GitHub`
```bash
$ cd ~/workspace/labs/	#переход в директорию workspace/labs/ 
$ export LAB_NUMBER=02	#в виртуальное окружение добавляем переменную LAB_NUMBER
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER} #клонируем репозиторий в папку
$ mkdir reports/lab${LAB_NUMBER} #созданаем директорию reports/lab
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md #копируем содержимое README в REPORT
$ cd reports/lab${LAB_NUMBER} #открываем директорию reports/lab
$ edit REPORT.md #открываем файл REPORT для редактирования
$ gistup -m "lab${LAB_NUMBER}" #делаем коммит
```

## Links

### Unix commands

- [ar](https://en.wikipedia.org/wiki/Ar_(Unix))
- [cat](https://en.wikipedia.org/wiki/Cat_(Unix))
- [cd](https://en.wikipedia.org/wiki/Cd_(command))
- [cp](https://en.wikipedia.org/wiki/Cp_(Unix))
- [cut](https://en.wikipedia.org/wiki/Cut_(Unix))
- [echo](https://en.wikipedia.org/wiki/Echo_(command))
- [env](https://en.wikipedia.org/wiki/Env_(shell))
- [ex](https://en.wikipedia.org/wiki/Ex_(editor))
- [file](https://en.wikipedia.org/wiki/File_(command))
- [find](https://en.wikipedia.org/wiki/Find)
- [ls](https://en.wikipedia.org/wiki/Ls)
- [man](https://en.wikipedia.org/wiki/Man_page)
- [mkdir](https://en.wikipedia.org/wiki/Mkdir)
- [mv](https://en.wikipedia.org/wiki/Mv)
- [nm](https://en.wikipedia.org/wiki/Nm_(Unix))
- [ps](https://en.wikipedia.org/wiki/Ps_(Unix))
- [pwd](https://en.wikipedia.org/wiki/Pwd)
- [rm](https://en.wikipedia.org/wiki/Rm_(Unix))
- [sed](https://en.wikipedia.org/wiki/Sed)
- [touch](https://en.wikipedia.org/wiki/Touch_(Unix))

### Package Managers

- [apt](http://help.ubuntu.ru/wiki/apt) | [dnf](https://en.wikipedia.org/wiki/DNF_(software)) | [yum](https://fedoraproject.org/wiki/Yum/ru)
- [brew](https://brew.sh) | [linuxbrew](http://linuxbrew.sh)
- [npm](https://docs.npmjs.com)

### Software

- [curl](https://www.gitbook.com/book/bagder/everything-curl/details)
- [wget](https://www.gnu.org/software/wget/manual/wget.pdf)
- [clang](https://clang.llvm.org)
- [g++](https://gcc.gnu.org/onlinedocs/gcc-4.0.2/gcc/G_002b_002b-and-GCC.html)
- [make](https://en.wikipedia.org/wiki/Make_(software))
- [open](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/open.1.html)
- [openssl](https://www.openssl.org)
- [nano](https://www.nano-editor.org)
- [tree](https://linux.die.net/man/1/tree)
- [vim](http://www.vim.org)

```
Copyright (c) 2017 Братья Вершинины
```
