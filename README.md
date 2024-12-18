# Plataforma de Telemedicina

Este é um projeto de uma plataforma de telemedicina desenvolvida com Django, permitindo que médicos e pacientes se cadastrem, façam login e interajam no sistema para agendar e realizar consultas online.

## Índice
- [Descrição](#Descrição)
- [Recursos](#Recursos)
- [Tecnologias Utilizadas](#Tecnologias_Utilizadas)
- [Pré-requisitos](#Pré-requisitos)
- [Instalação](#Instalação)
- [Uso](#Uso)
- [Contribuição](#Contribuição)
- [Licença](#Licença)

## Descrição
Este projeto é uma plataforma de telemedicina onde médicos e pacientes podem se registrar e interagir para realizar consultas. O sistema foi desenvolvido usando Django e fornece as funcionalidades para agendamento de consultas e videochamadas.

-  __Médicos:__ Podem se cadastrar, fornecer credenciais profissionais, cadastrar horários disponíveis para consultas, visualizar consultas agendadas e realizar videochamadas com os pacientes.

-  __Pacientes:__ Podem se cadastrar, escolher especialidades, visualizar médicos disponíveis, agendar consultas e se conectar com os médicos via videochamada.

## Recursos
-  __Cadastro e login de usuários:__  Tanto médicos quanto pacientes podem se cadastrar e realizar login.
  
-  __Cadastro de médicos:__ Médicos devem fornecer credenciais e especialidades.
  
-  __Agendamento de consultas:__ Pacientes escolhem médicos e marcam consultas com base nos horários disponíveis.
  
-  __Visualização de consultas:__ Médicos podem visualizar as consultas agendadas e entrar em videochamadas.
  
-  __Videochamada:__ Funcionalidade para médicos e pacientes interagirem em tempo real através de videochamadas.

## Tecnologias Utilizadas
-  __Django__
  
-  __Django Rest Framework__
  
-  __SQLite__ (banco de dados local)

-  __HTML/CSS/JavaScript__ para a interface do usuário

## Pré-requisitos
Antes de começar, você precisará ter as seguintes ferramentas instaladas:
-  __Python 3.x__
-  __Git__
  
Além disso, recomenda-se usar um ambiente virtual Python para gerenciar dependências.

## Instalação
1. Clone o repositório para sua máquina local:

    ```
    git clone https://github.com/seu-usuario/nome-do-repositorio.git
    cd nome-do-repositorio
    ```

2. Crie e ative um ambiente virtual:

    ```
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    ```

3. Instale as dependências do projeto:

    ```
    pip install -r requirements.txt
    ```

4. Execute as migrações do banco de dados:

    ```
    python manage.py migrate
    ```

5. Inicie o servidor de desenvolvimento:

    ```
    python manage.py runserver
    ```

6. Acesse o sistema em http://127.0.0.1:8000/ no seu navegador.

## Uso

Para utilizar o sistema é necessário realizar um cadastro, registrando apenas usuário, email e senha.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/00a.png">

Após o cadastro, é preciso fazer login para ter acesso a sua própria sessão de usuário.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/00.png">

Se o usuário for médico, em sua home, é possível visualizar também todos os outros médicos cadastrados e suas especialidades.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/01.png">

É possível realizar um filtro para localizar um médico cadastrado de acordo com sua especialidade. Esta função está disponível para médicos ou pacientes realizarem o filtro.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/02.png">

É possível realizar um filtro para localizar um médico cadastrado de acordo com o seu nome ou partes do nome. Esta função está disponível para médicos ou pacientes realizarem o filtro.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/03.png">

O médico cadastrado pode abrir horários para consultas.

<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/04.png">

É possível o médico visualizar todas as suas consultas e seus status.
<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/04.png">
Quando chega o dia e horário da consulta, o médico adiciona o link da videoconferência e inicia a consulta.
<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/06.png">
Quando uma consulta é finalizada com um paciente, o médico também pode publicar documentos como atestado médico, receitas, exames etc.
<img src = "https://github.com/allesantos/allesantos/blob/main/imagens/Telemedicina-Django/07.png">

## Contribuição
Sinta-se à vontade para contribuir com este projeto. Siga estas etapas:

1. Faça um fork do repositório.

2. Crie uma nova branch para sua feature/bugfix:

```
git checkout -b minha-feature
```

3. Envie suas alterações:

```
git push origin minha-feature
```

4. Abra um Pull Request.

## Licença
Este projeto está licenciado sob a Licença MIT. Consulte o arquivo LICENSE para mais informações.
