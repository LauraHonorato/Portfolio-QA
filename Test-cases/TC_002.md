## 🧪 Caso de Teste: Paginação em Bebês > Balanço & Baby Bouncer

### 🆔 Identificação
- **ID:** TC_002
- **Módulo:** Pesquisa e Listagem de Produtos
- **Tipo:** Teste funcional / Exploratória
- **Prioridade:** Alta

---

### 🌐 Cenário de Teste
Verificar que todas as páginas de resultados na categoria **Bebês > Balanço & Baby Bouncer** exibam produtos corretamente sem apresentar a mensagem de erro de "nenhum resultado".

---

### 📝 Dados de Entrada
| Parâmetro                        | Valor                                                         |
|----------------------------------|---------------------------------------------------------------|
| Categoria                        | Bebês                                                         |
| Subcategoria                     | Balanço & Baby Bouncer                                        |
| Páginas                          | 1 a última página conforme paginação (ex: 1, 2, 3, 4, ..., n) |

---

### ✅ Resultado Esperado
- Cada página de 1 a n deve listar produtos sem apresentar mensagem de erro.
- A quantidade de produtos exibidos por página deve corresponder ao padrão definido (ex: 24 itens).

---

### ⛔ Resultado Obtido
- Páginas específicas (3, 8, 9) exibem a mensagem de erro "Ooops... não encontramos resultados".

---

### 🚀 Passos para Execução
1. Acessar `(https://www.zoom.com.br/baby-bouncer-e-cadeira-de-balanco)`
2. Confirmar total de resultados e número de páginas.
3. Navegar sequencialmente pelas páginas de 1 até n.
4. Verificar se alguma página exibe mensagem de erro.

---

### 📊 Evidências
- Capturas de tela das páginas com erro
- Captura de tela de páginas sem erro para comparação
- Vídeo-captura de telas

---

### 🚩 Status
**Falha**: Páginas 3, 8, 9 (e outras) exibem erro indevido, indicando falha de paginação.
As páginas não possuem um número N definido para retorno dos resultados,em algumas páginas, por exemplo a página 4, o retorno é somente 1 resultado, mesmo tendo a página 5 em sequência, enquanto a página 7 retorna mais de 7 resultados. 

---

### 💡 Observações
- Validar após correção com script automatizado que percorre todas as páginas.
