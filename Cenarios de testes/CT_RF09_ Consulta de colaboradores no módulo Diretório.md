## Cenário 09: Consulta de colaboradores no módulo Diretório.

### Caso de Teste 01: Buscar colaborador por nome com sucesso.

| ID       | Descrição                                                               |
| :------- | :---------------------------------------------------------------------- |
| C09-CT01 | O sistema deve retornar corretamente o colaborador pesquisado pelo nome. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** insere o nome de um colaborador existente no campo de busca |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** o sistema deve exibir o colaborador correspondente à busca |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O nome, cargo e localização do colaborador devem ser exibidos corretamente. |

---

### Caso de Teste 02: Buscar colaborador inexistente.

| ID       | Descrição                                                                   |
| :------- | :-------------------------------------------------------------------------- |
| C09-CT02 | O sistema deve exibir uma mensagem apropriada quando nenhum colaborador for encontrado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** digita um nome que não corresponde a nenhum colaborador    |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** uma mensagem como \"No Records Found\" deve ser exibida |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir claramente que não há registros encontrados. |

---

### Caso de Teste 03: Aplicar filtro por cargo (Job Title).

| ID       | Descrição                                                                |
| :------- | :------------------------------------------------------------------------ |
| C09-CT03 | O sistema deve permitir a filtragem de colaboradores por cargo.           |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e o sistema deve conter dados de funcionários. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** seleciona um cargo no campo \"Job Title\"                 |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** apenas os colaboradores com o cargo selecionado devem ser listados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O filtro deve funcionar corretamente e retornar apenas resultados válidos. |

## 🔗 Evidências (Jam.dev)

- **C01-CT01** → [Execução](https://jam.dev/c/56c680fd-ab5d-4e80-ba0e-f8e3851f4669)  
- **C01-CT02** → [Execução](https://jam.dev/c/3c38ace6-c123-4fa2-9e6b-13cda270cc09)  
- **C01-CT03** → [Execução](https://jam.dev/c/601a35d6-7f7d-46b4-9bb6-bf153a40b6ef)
