CICATRIZES FICHA - VERSAO CORRIGIDA PARA OWLBEAR RODEO

POR QUE A VERSAO ANTERIOR FALHOU
- O manifesto antigo usava estrutura errada com "actions".
- Depois, a rota do popover pode ter ficado inconsistente no ambiente do Owlbear.
- Esta nova versao usa index.html na raiz, o que se aproxima mais do fluxo comum de extensoes publicadas.

ARQUIVOS DESTA VERSAO
- manifest.json
- index.html
- icon.svg

MANIFESTO USADO
{
  "name": "Cicatrizes Ficha",
  "version": "1.0.1",
  "manifest_version": 1,
  "action": {
    "title": "Cicatrizes Ficha",
    "icon": "icon.svg",
    "popover": "index.html",
    "height": 700,
    "width": 460
  }
}

COMO SUBSTITUIR NO GITHUB
1. Apague o ficha.html antigo se quiser evitar confusao.
2. Envie estes novos arquivos para a raiz do repositorio.
3. Confirme que a URL abaixo abre no navegador:
   https://SEU-USUARIO.github.io/fichas/index.html
4. Confirme tambem:
   https://SEU-USUARIO.github.io/fichas/manifest.json
5. Reinstale a extensao no Owlbear Rodeo.

SE AINDA DER ERRO
- Teste trocar icon e popover para URLs absolutas completas.
- Se mesmo assim falhar, o proximo passo deve ser usar Vite, como extensoes mais maduras fazem.
