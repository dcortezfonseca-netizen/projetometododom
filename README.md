# Método DOM — Diagnóstico Empresarial 360°

Aplicativo de página única (HTML/CSS/JS, sem build) para o diagnóstico de risco jurídico, tributário e estrutural da Cortez Fonseca Advogados.

## Uso

Abra `index.html` diretamente no navegador, ou sirva a pasta com qualquer servidor estático. Não há dependências nem etapa de build.

- **Cliente**: responde ao perfil da empresa e às perguntas por pilar; ao final, recebe o relatório com score, mapa de riscos e plano de ação.
- **Consultor**: acesse com `?modo=consultor` na URL para ver, além do relatório do cliente, a leitura comercial (honorários sugeridos, roteiro de devolutiva) e para reconstruir o diagnóstico de um lead colando o JSON completo recebido por e-mail/planilha.

## Configuração

Edite o bloco `CONFIG` no topo do `<script>` em `index.html`: WhatsApp, e-mail do consultor, URL do webhook (Google Apps Script) que recebe cada diagnóstico concluído.

## Privacidade

Respostas e progresso ficam salvos apenas em `localStorage` no navegador do respondente até o envio. O envio ao consultor usa o webhook configurado (dados tratados nos termos da LGPD, conforme texto do próprio relatório).
