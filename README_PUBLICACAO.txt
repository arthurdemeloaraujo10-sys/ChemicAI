CHEMICAI. — LDMF-4/7 3.7V
Cérebro central + PWA + publicação

1) SUPABASE
- Abra o projeto Supabase.
- Authentication > Users > Add user: crie sua conta administradora com o e-mail configurado no projeto.
- Confirme o usuário se seu projeto exigir confirmação de e-mail.
- Abra SQL Editor > New query.
- Abra o arquivo supabase_schema.sql deste ZIP, copie tudo, cole no SQL Editor e clique Run.
- Em seguida, abra o arquivo ChemicAI_LDMF_4_7_3_7V.html e substitua:
  COLE_AQUI_SUA_PUBLISHABLE_KEY
  pela sua Publishable/anon key.
- A URL do projeto já está configurada neste pacote.
- NÃO coloque service_role ou sb_secret no HTML.

2) TESTE LOCAL
- Não abra por file:// se quiser testar o PWA/service worker.
- Use um servidor HTTPS/localhost. Uma forma simples é publicar no GitHub Pages e testar pelo endereço publicado.

3) GITHUB PAGES
- Crie um repositório público chamado ChemicAI.
- Envie os arquivos deste ZIP (não envie o ZIP como único arquivo):
  ChemicAI_LDMF_4_7_3_7V.html
  manifest.webmanifest
  sw.js
  icon-192.png
  icon-512.png
- Renomeie ChemicAI_LDMF_4_7_3_7V.html para index.html antes de publicar OU ajuste o start_url do manifest para o nome atual.
- GitHub > Settings > Pages > Deploy from a branch > main > /(root) > Save.

4) GOOGLE SITES
- Publique primeiro o ChemicAI em uma URL HTTPS.
- No Google Sites: Inserir > Incorporar > Por URL.
- Cole a URL do ChemicAI publicado.
- Publique o Google Sites.

5) DOMÍNIO PRÓPRIO
- Depois de o site funcionar, registre seu domínio no Registro.br ou outro registrador.
- Aponte o domínio para a hospedagem escolhida.

6) COMO O CÉREBRO FUNCIONA
- Visitante: somente Análise.
- Administrador: Análise + Treinamento + Memória.
- RLS no Supabase impede escrita/edição/exclusão por visitantes.
- O conhecimento central fica no Supabase e é carregado pelos dispositivos.
- Imagens são armazenadas no bucket chemicai-images.

7) OBSERVAÇÃO
- O mecanismo atual de raciocínio do projeto continua sendo um sistema de comparação de vetores visuais/textuais/características. Ele não é uma rede neural/foundation model real e não confirma composição química laboratorial pela aparência.
