## 🔢 Caso de Teste: Reserva com 2 adultos + 2 crianças no site da rede Nacional Inn

### 📝 Identificação
- **ID:** TC_001
- **Módulo:** Reserva Online
- **Tipo:** Teste funcional / exploratório
- **Prioridade:** Alta

---

### 🌐 Cenário de Teste
**Verificar se é possível realizar a reserva de um quarto para 2 adultos e 2 crianças pequenas diretamente no site do hotel, conforme disponibilidade informada por plataformas parceiras (ex: Booking.com).**

---

### 🛋 Dados de Entrada
| Parâmetro             | Valor                     |
|------------------------|---------------------------|
| Quantidade de adultos | 2                         |
| Quantidade de crianças| 2 (com idades 01 e 06 anos)   |
| Datas da reserva      | [26/07/2025 a 01/08/2025] |
| Plataforma            | Site e App oficiais do hotel     |

---

### ✅ Resultado Esperado
- O sistema deve **oferecer quartos compatíveis** com a ocupação total de 2 adultos e 2 crianças.
- A seleção de **apenas 1 quarto** deve ser possível, caso esse tipo de ocupação seja permitido (verificado na Booking).
- Nenhuma mensagem de erro bloqueando a reserva deve ser exibida **se o mesmo é permitido via plataformas parceiras**.

---

### ❌ Resultado Obtido (até o momento)
- O site oficial do hotel exige a seleção de **2 quartos separados**, informando que os quartos disponíveis não comportam os 4 hóspedes.
- A Booking.com permite normalmente a seleção de 1 quarto para a mesma configuração.

---

### 📅 Passos para Execução
1. Acessar o site oficial e também o aplicativo da rede Nacional Inn
2. Inserir datas de entrada e saída
3. Selecionar "2 adultos e 2 crianças"
4. Clicar em "Buscar disponibilidade"
5. Verificar opções de quarto apresentadas

---

### 📊 Evidências esperadas
- Prints da tela de erro (disponíveis em "evidências")
- Comparativo com a Booking ou outras plataformas

---

### 🚀 Status
**Falha**: bloqueio indevido para configuração válida

### 🧠 Sugestão
Revisar regra de ocupação no motor de reservas para garantir alinhamento com parceiros terceiros e evitar perda de conversões.
