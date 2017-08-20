# sara-web
Em progresso...

## Começando

Essas instruções irão te orientar na cópia do projeto em funcionamento na sua máquina local para fins de desenvolvimento e testes. Veja a inserção de notas sobre como implantar o projeto em um sistema real.

### Pré-requisitos

O que você precisa para instalar o software e como instalá-lo

```
Python 3.5 ou superior

Você precisa instalar um BD(SqLite, PostgreSQL) à sua escolha para criar as tabelas e invocar serviços.
```

> Você precisa ver um curto (e muito bom) tutorial sobre Python e Django [aqui](https://tutorial.djangogirls.org/).
  No tutorial Django Girls você encontrará passos específicos para seu sistema operacional.

### Instalando

Criar o python virtualenv

```
python3 -m venv myvenv
```

Ativar o virtualenv

```
source myvenv/bin/activate
```

Instale os requisitos do projetos, salvos em requirements.txt

```
pip install -r requirements.txt
```

### Inicializar o Esquema do Banco de Dados

Crie arquivos de migração, executando:

```
python manage.py makemigrations manager
```

e, em seguida, aplique-os:

```
python manage.py migrate
```

### Inicializar Dados Padrão
> Esta seção é opcional. Apenas execute os comandos abaixo se você quer carregar um conjunto de dados padrão.

Execute o comando abaixo para carregar os dados iniciais:

```
python manage.py loaddata manager/fixtures/initial_data.json
```

Se você executou esses comandos acima, você pode usar um super usuário padrão. Veja a próxima seção e use esta esses dados:

- usuário: admin
- senha: @dmin123


### Executando

Você irá precisar criar um usuário com altas permissões, chamado "super usuário". Para criar um super usuário, execute:

```
python manage.py createsuperuser
```

Execute o principal módulo python

```
python manage.py runserver
```


## Autores

Veja também a lista de [contribuidores](https://github.com/icarojerry/sara/contributors) que participaram deste projeto.

## Licença

Este projeto está licenciado sobre a GPL-3.0 License - veja a [LICENÇA](LICENÇA) arquivo para detalhes.
