# Entidades [BANCO] `MyseumDB` (v0.0.1)

## [TABELA] `jogos`

* Id
* Nome
* Plataformas
* Cadastro de jogos.
* Plataformas.
* Desenvolvedoras.
* Gêneros.
* Screenshots.
* Histórico de versões.
* Data de lançamento
* Data Postado
* fk_id_usuario (quem fez o post do game)

## [TABELA] `usuarios`

* Id
* Username
* Email
* Senha
* Favoritos

## [TABELA] `favoritos`

* Id
* fk_id_jogo
* fk_id_usuario
* data_favoritado

---

# Relacionamentos

*`1` [POSTAR]*

`JOGOS` --POSTAR--> `USUARIOS` 
  (0, N)              (1, 1)

> Um usuário pode postar vários games, porém um game só pode ser postado por um usuário.    

*`2` [FAVORITAR]*

`JOGOS` --FAVORITAR--> `USUARIOS` 
  (0, N)                 (0, N)

> Um usuário pode favoritar um ou mais games e um game pode ser favoritado por um ou mais usuários.

---

# Observações

Este documentos foi escrito 100% sem uso de IA, como pode perceber está em um nível de júnior mesmo :).

Alem disso, se trata da arquitetura do Myseum versao 0.0.1, então não esta rubusta.

obrigado.