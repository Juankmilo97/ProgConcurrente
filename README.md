# ProgConcurrente

Tutorial del Paradigma de Programación Concurrente usando Golang

## Guía de Instalación

### Pre-requisitos

- [Go 1.9+](https://golang.org/doc/install) - including GOPATH/bin added to your PATH (i.e., you can run Go binaries that you `go install`).
- [Jupyter Notebook](http://jupyter.readthedocs.io/en/latest/install.html) or [nteract](https://nteract.io/desktop)
- [ZeroMQ 4.X.X](http://zeromq.org/intro:get-the-software) - for convenience, pre-built Windows binaries (v4.2.1) are included in the zmq-win directory.
- [pkg-config](https://en.wikipedia.org/wiki/Pkg-config)

### Pasos de instalación

1) Descargue el compilador de Go de https://golang.org/dl/

2) Descomprimalo ($HOME/gocompiler/)

3) Cree un nuevo directorio para su proyecto de Go ($HOME/golexamples/myproject1)

4) Añada las siguientes lineas a su archivo $HOME/.bashrc (nano ~/.bashrc)


export GOROOT=$HOME/gocompiler/go
export PATH=$GOROOT/bin:$PATH

export GOPATH=$HOME/mygoproject1
export PATH=$GOPATH/bin:$PATH

5) Para obtener la ayuda de los comandos de Go

go help

6) Verifique que la versión sea superior a 9.x

pip —version

7) Actualice el paquete de python-pip

sudo pip install —upgrade pip

8) Instale Jupyter

sudo pip install jupyter

9) Corra el servidor de Jupyter para probar que la instalación fue exitosa

jupyter notebook

10) Instalar goimports

go get golang.org/x/tools/cmd/goimports

11) Instalar ZeroMQ

sudo apt-get install libzmq3-dev

12) Instaler golang kernel

go get -tags zmq_4_x github.com/gopherds/gophernotes

13) Cree un directorio para la configuración del nuevo kernel

mkdir -p ~/.local/share/jupyter/kernels/gophernotes

14) Copie la configuración del kernel dentro del directorio .ipython

cp -r $GOPATH/src/github.com/gopherds/gophernotes/kernel/* ~/.local/share/jupyter/kernels/gophernotes

15) Arranque el servidor de Jupyter y cree un Notebook de Go

jupyter notebook

