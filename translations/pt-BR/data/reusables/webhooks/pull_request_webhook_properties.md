| Tecla  | Tipo     | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| ------ | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Ação` | `string` | A ação que foi executada. Pode ser  `opened`, `edited`, `closed`, `assigned`, `unassigned`, `review_requested`, `review_request_removed`, `ready_for_review`, `labeled`, `unlabeled`, `synchronize`, `locked`, `unlocked` ou `reopened`. Se a ação é `closed` e a chave `merged` é `false`, o pull request foi fechado com commits não mesclados. Se a ação for `closed` e a chave `merged` for `verdadeira`, o pull request foi mesclado. |