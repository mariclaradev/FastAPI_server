Este script cria um servidor FastAPI para autenticação na API de um aplicativo e permite reiniciar automaticamente um bot no Heroku caso ocorra falha no login.

🔹 Principais Funcionalidades:
✅ Autenticação – Faz login na API do Amino, gerando um ID de dispositivo único e assinando os dados com HMAC-SHA1.
✅ Reinício Automático – Se o login falhar, o bot é reiniciado via Heroku API.
✅ Servidor FastAPI – Oferece endpoints /login (para autenticação) e /reset (para reiniciar o bot).
✅ User-Agent Aleatório – Evita bloqueios na API ao gerar cabeçalhos dinâmicos.

🔹 Principais Bibliotecas Utilizadas:

FastAPI → Cria o servidor web.
requests → Envia requisições HTTP para a API do Amino.
heroku3 → Gerencia e reinicia o bot no Heroku.
hmac, sha1, base64 → Protegem a autenticação com assinatura digital.
names, random, socket, uuid → Geram identificadores únicos para o dispositivo.
Esse script facilita a automação de login e gerenciamento de um bot, garantindo um funcionamento contínuo e seguro.
