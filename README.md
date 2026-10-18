# Site-educacional
Plataforma web educacional gratuita para consulta de conteúdos do Ensino Fundamental e do Ensino Médio.  

# Plataforma Educacional

## 1. Sobre o projeto

A Plataforma Educacional é um sistema web que tem como objetivo disponibilizar conteúdos escolares gratuitos do Ensino Fundamental e do Ensino Médio.

O sistema permitirá que os usuários acessem os níveis de ensino e consultem conteúdos educacionais organizados por matéria, facilitando a busca por informações e materiais de estudo.

A plataforma também contará com administradores responsáveis pelo gerenciamento dos conteúdos disponibilizados.

## 2. Objetivo

Desenvolver um sistema web educacional que facilite o acesso a conteúdos escolares gratuitos, organizados de acordo com o nível de ensino e a matéria correspondente.

## 3. Funcionalidades principais

- Cadastro e identificação de usuários.
- Acesso dos alunos aos níveis de ensino.
- Consulta de conteúdos educacionais.
- Organização dos conteúdos por nível de ensino e matéria.
- Gerenciamento dos conteúdos pelos administradores.

## 4. Requisitos 

- **R01:** O sistema deve armazenar os dados dos usuários.
- **R02:** O sistema deve distinguir alunos e administradores.
- **R03:** O sistema deve permitir que os alunos acessem os níveis de ensino.
- **R04:** O sistema deve disponibilizar conteúdos educacionais associados aos níveis de ensino.
- **R05:** O sistema deve permitir a consulta dos conteúdos por matéria.
- **R06:** O sistema deve permitir que os administradores gerenciem os conteúdos.

## 5. Regras

- **R01:** A plataforma será destinada à disponibilização de conteúdos do Ensino Fundamental e do Ensino Médio.
- **R02:** Os usuários serão classificados como alunos ou administradores.
- **R03:** Os alunos estarão relacionados aos níveis de ensino por meio do relacionamento Pertence.
- **R04:** Os níveis de ensino estarão relacionados aos conteúdos por meio do relacionamento Possui.
- **R05:** Cada conteúdo estará associado a um nível de ensino.
- **R06:** Os administradores serão responsáveis pelo gerenciamento dos conteúdos.
- **R07:** Os conteúdos terão título, descrição e matéria.

## 6. Modelo Entidade-Relacionamento (MER)

O modelo conceitual do banco de dados é composto pelas seguintes entidades:

### Usuário
Armazena as informações gerais dos usuários, incluindo identificador, nome, e-mail e senha.

### Aluno
Representa o usuário que acessa os níveis de ensino e consulta os conteúdos educacionais. Possui o atributo matrícula.

### Administrador
Representa o usuário responsável pelo gerenciamento dos conteúdos da plataforma. Possui o atributo código_administrador

### Nível de Ensino
Representa os níveis escolares disponibilizados pelo sistema, como Ensino Fundamental e Ensino Médio.

### Conteúdo
Armazena os materiais educacionais disponibilizados na plataforma, incluindo identificador, título, descrição e matéria.

### Relacionamentos

- **Pertence:** relaciona os alunos aos níveis de ensino.
- **Possui:** relaciona os níveis de ensino aos conteúdos.
- **Admin_conteúdo (Gerencia):** representa o gerenciamento dos conteúdos pelos administradores.

A entidade Usuário é especializada em Aluno e Administrador, permitindo que os dois tipos compartilhem os atributos gerais de usuário.

### Imagem do modelo conceitual

![Modelo Entidade-Relacionamento do Banco Escolar](mer-banco-escolar.png)


## 7. Tecnologias

- Modelagem conceitual do banco de dados: brModelo 3.2.
- Sistema web e banco de dados: a definir.

## 8. Status do projeto

Projeto acadêmico em desenvolvimento, com o modelo conceitual do banco de dados elaborado.

## 9. Autor
- João Gabriel
- Caio
