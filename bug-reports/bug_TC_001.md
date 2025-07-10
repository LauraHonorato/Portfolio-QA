## 🐞 **[BUG] Reserva incorreta para 2 adultos + 2 crianças no site e App Nacional Inn**

### 🔍 **Descrição do problema**
Ao tentar realizar uma reserva diretamente pelo site e pelo App da rede Nacional Inn para **2 adultos e 2 crianças pequenas**, o sistema **bloqueia a seleção de apenas um quarto**, alegando que a ocupação excede o limite permitido.

Porém, ao realizar o mesmo processo na plataforma **Booking.com**, é possível finalizar a reserva **com um único quarto**, para as **mesmas pessoas**, no **mesmo hotel e datas**.

Isso sugere uma **inconsistência na lógica de verificação de ocupação**, que pode estar prejudicando a experiência do usuário e gerando perda de conversões diretas para o hotel.

---

### ✅ **Resultado esperado**
- O site/App do hotel deveria permitir a reserva de **1 quarto** para **2 adultos + 2 crianças**, desde que essa configuração seja suportada pelas acomodações (como já ocorre na Booking.com).

---

### ❌ **Resultado obtido**
- O sistema exibe a mensagem:  
  *“Para acomodar 4 pessoas você precisará escolher mais de um quarto.”*
- Bloqueia a continuidade da reserva com apenas 1 quarto, mesmo para crianças pequenas acompanhadas de adultos.

---

### 📱 **Ambiente de testes**
- Dispositivo: Android / Google Chrome
- Data do teste: 09/07/2025
- Site testado: https://nacionalinn.letsbook.com.br/reserva e Aplicativo disponível na Play Store
- Plataforma de comparação: https://www.booking.com

---

### 📸 **Evidências**
- [x] Screenshot da mensagem de erro no site do hotel  
- [x] Screenshot da confirmação da reserva normal na Booking.com  
- [x] Print da configuração usada (2 adultos + 2 crianças)

---

### 🧪 **Tipo de teste aplicado**
- [x] Teste funcional  
- [x] Teste de lógica de negócios  
- [x] Teste de consistência entre plataformas  
- [x] Teste de UX (experiência do usuário)

---

### 🧠 **Impacto estimado**
- Perda de reservas diretas para o hotel  
- Experiência negativa e confusa para o usuário  
- Risco de inconsistência com canais terceiros (Booking, Expedia, etc.)  
- Dificuldade para famílias viajando com crianças

---

### 💡 **Sugestão de melhoria**
- Revisar lógica de ocupação do motor de reservas  
- Garantir que crianças pequenas sejam consideradas corretamente dentro da política do quarto  
- Realizar teste de regressão após ajustes
