# Nexo — IA no dia a dia e a promoção da paz

Aplicativo web responsivo para a feira de ciências. O mesmo endereço funciona em celulares, tablets e computadores. A interface conversa com o servidor, que envia as perguntas à Gemini API; a chave fica no servidor e nunca no navegador.

## Publicar para compartilhar

O projeto está pronto para o Render:

1. Coloque esta pasta em um repositório GitHub.
2. No Render, escolha **New → Blueprint** e conecte o repositório. O arquivo `render.yaml` configura o serviço.
3. Crie uma chave no Google AI Studio e, nas variáveis de ambiente do serviço Render, defina `GEMINI_API_KEY`. Não publique essa chave no GitHub nem a envie no grupo.
4. Faça o deploy e compartilhe o endereço `https://...onrender.com` com a turma.

O plano gratuito do Render pode colocar o servidor em repouso após inatividade; a primeira abertura depois disso pode demorar. O Google AI Studio oferece cota gratuita para alguns modelos, incluindo `gemini-3.6-flash`, sujeita a limites que podem mudar. No nível gratuito, o conteúdo enviado pode ser usado pelo Google para melhorar seus produtos. Não digite dados pessoais ou informações privadas no app. Confira os limites atuais antes de apresentar.

## Executar localmente

Requer Node.js 20 ou superior. Crie uma chave no Google AI Studio. No terminal, dentro desta pasta:

```powershell
$env:GEMINI_API_KEY="sua-chave"
npm start
```

Abra `http://localhost:3000`. Cada participante precisaria rodar o servidor e ter uma chave para usar localmente; para compartilhar com a feira, use a publicação e um único servidor configurado.

## Sobre o Nexo

O assistente responde em português brasileiro, explica usos cotidianos da IA, explora oportunidades para diálogo e cooperação e também aborda riscos como vieses, desinformação, vigilância, privacidade e uso em armas. Foi instruído a admitir incerteza e a lembrar que tecnologia não substitui decisões humanas.
