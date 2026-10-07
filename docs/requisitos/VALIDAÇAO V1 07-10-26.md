# CONTROLE DE ESTOQUE — NTI / SR-DF

**Projeto:** Sistema de Controle de Estoque

**Setor:** Núcleo de Tecnologia da Informação — NTI / SR-DF

**Responsável pelo levantamento:** Davi

**Contato/Responsável do setor:** Jonathan

**Data:** 08/10/2026

**Tecnologia prevista:** Oracle APEX + Oracle Database

---

## 1. CATEGORIAS E MODELOS

O sistema permitirá criar e manter categorias e modelos de equipamentos.

**Exemplos de categorias:**

- Notebook
- Desktop
- Periféricos
- Memória RAM
- Outras categorias que a NTI precisar

**Exemplo de modelo:**

- Categoria: Notebook
- Marca: Lenovo
- Modelo: ThinkPad T480

Ao cadastrar um equipamento, o usuário poderá selecionar o modelo já existente, evitando preencher novamente as informações do modelo.

**OBS:**
```

```

## 2. EQUIPAMENTOS

Cada equipamento físico terá seu próprio cadastro.

**Informações principais:**

- Modelo
- Patrimônio
- Número de série
- Situação
- Observação
- Data de entrada/cadastro

Quando estiver em uso:

- Nome da pessoa
- Matrícula
- Setor

O sistema deverá permitir consultar, por exemplo, todos os ThinkPad T480 e saber quantos existem e qual a situação de cada um.

**OBS:**
```

```

## 3. SITUAÇÃO DO EQUIPAMENTO

Situações previstas na V1:

- **Disponível** — está no estoque e pode ser utilizado.
- **Em uso** — está com uma pessoa.
- **Em manutenção** — está sendo analisado ou reparado.
- **Descarte** — não será mais utilizado.

A localização física não será controlada, pois o estoque está concentrado na sala da NTI.

**OBS:**
```

```

## 4. MOVIMENTAÇÕES

O sistema manterá o histórico das movimentações dos equipamentos.

**Principais movimentações:**

- Entrada
- Saída
- Devolução
- Manutenção
- Descarte

Cada movimentação poderá registrar:

- Equipamento
- Tipo de movimentação
- Data e hora
- Pessoa relacionada, quando necessário
- Usuário que realizou o registro
- Observação

**OBS:**
```

```

## 5. FLUXO DE MANUTENÇÃO / DEVOLUÇÃO

Quando um equipamento chegar com problema:

**Entrada → Avaliação/Manutenção → Decisão**

Se for recuperado:

- volta para o estoque como disponível; ou
- é devolvido à pessoa.

Se não for recuperável:

- vai para descarte.

A manutenção poderá registrar:

- Quem realizou
- O que foi feito
- Observações

**OBS:**
```

```

## 6. ENTREGA / SAÍDA DE EQUIPAMENTO

Quando uma pessoa precisar de um equipamento:

**Consultar estoque → selecionar equipamento disponível → registrar saída → vincular à pessoa → equipamento fica "Em uso".**

A saída terá:

- Equipamento
- Pessoa
- Data e hora
- Usuário responsável pelo registro
- Observação

O equipamento antigo da pessoa poderá seguir para manutenção/avaliação.

**OBS:**
```

```

## 7. CONSULTA E HISTÓRICO

O sistema deverá permitir consultar:

- Equipamentos disponíveis
- Equipamentos em uso
- Equipamentos em manutenção
- Equipamentos em descarte
- Quantidade por modelo
- Equipamentos de uma determinada pessoa
- Histórico de movimentações

Cada equipamento deverá possuir seu próprio histórico.

**OBS:**
```

```

## 8. USUÁRIOS E ACESSOS

### Administrador

Acesso a todas as funcoes.

### Usuário

Acesso às operações do dia a dia da NTI, como:

- Cadastro de modelos
- Cadastro de equipamentos
- Consultas
- Entradas
- Saídas
- Devoluções
- Manutenção
- Descarte
- Histórico

**OBS:**
```

```

# FUNCIONALIDADES FUTURAS — FORA DA V1

Estas funcionalidades não fazem parte da primeira versão, mas poderão ser adicionadas posteriormente:

- Integração com **E-LOG** para preenchimento automático dos dados dos equipamentos.
- Integração com **EGP** para identificação automática das pessoas.
- Busca automática de equipamentos por patrimônio.
- Busca automática de pessoas.
- Outras automações conforme a necessidade da NTI.

**OBS:**
```

```