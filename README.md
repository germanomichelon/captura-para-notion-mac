# Captura para Notion — Mac

O app **Captura para Notion** para Mac, pronto para instalar: captura rápida para um database do
Notion que funciona sem internet. A nota (com fotos, arquivos e áudio) fica no Mac até a página ser
criada **e conferida** no Notion. ⌃⌥N abre a captura por cima de qualquer app; notas de voz são
transcritas no próprio Mac pelo Whisper.

O código fica num repositório privado; aqui saem só as versões prontas, para os Macs se
atualizarem sozinhos.

## Instalar

No Terminal:

```bash
curl -fL -o /tmp/captura.zip https://github.com/germanomichelon/captura-para-notion-mac/releases/latest/download/CapturaParaNotion-mac.zip && ditto -x -k /tmp/captura.zip /Applications && open "/Applications/Captura para Notion.app"
```

Pelo navegador também dá: baixe `CapturaParaNotion-mac.zip` da versão mais nova, abra e arraste o
app para Aplicativos. Como o app não é notarizado pela Apple, a primeira abertura é bloqueada —
Ajustes do Sistema → Privacidade e Segurança → "Abrir Mesmo Assim" (uma vez só).

Depois, nas Configurações do app: o token da integração do Notion, o database e, para transcrever
notas de voz, "Baixar o Whisper (1 GB)".

## Atualizações

O app confere esta página a cada 6 horas e se atualiza sozinho, quando você não estiver usando —
sem token nem conta. Cada versão vem com um `.sig`: a assinatura feita com uma chave que só existe
no Mac onde o app é desenvolvido. Versão sem a assinatura certa é recusada.

Requer macOS 14 ou mais novo, em Mac com Apple Silicon.
