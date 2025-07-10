## 🐞 [BUG] Paginação inconsistente em categoria Bebês > Balanço

### 🔍 Descrição
Na categoria **Bebês > Baby Bouncer e Cadeira de Balanço** do site Zoom, a busca retorna **~260 resultados** e gera paginação automática.  
Em páginas como **3, 8 e 9**, o site exibe a mensagem de erro:  
> “Ooops… não encontramos resultados para sua busca…”  
Mesmo havendo itens a serem mostrados, e outras páginas (4, 10) funcionarem normalmente.

### ✅ Resultado Esperado
- Todas as páginas de 1 a N devem exibir o subconjunto correto de produtos.
- Nunca deve apresentar mensagem de “nenhum resultado” quando há itens disponíveis.

### ❌ Resultado Obtido
- Páginas 3, 8, 9 (e eventualmente outras) retornam erro de “nenhum resultado”.

### 📱 Ambiente
- Navegador: Chrome (desktop e mobile)  
- URL base: https://www.zoom.com.br/baby-bouncer-e-cadeira-de-balanco
- Data do teste: [10/07/2025]

### 🧪 Tipo de Teste
- Teste funcional (paginação)  
- Teste de consistência de conteúdo  
- Teste de UX (mensagem de erro indevida)

### 💡 Sugestão
- Ajustar lógica de paginação para recalcular corretamente o total de páginas.  
- Garantir fallback que mostre a página anterior (ou redirecione ao início) em vez de exibir erro.
