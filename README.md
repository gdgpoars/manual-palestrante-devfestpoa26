# Manual da Pessoa Palestrante — DevFest Porto Alegre 2026

Site único (HTML/CSS/JS, sem build) com o manual oficial para quem vai palestrar no
DevFest Porto Alegre 2026 (31/10/2026, Faculdade Dom Bosco).

## O que tem aqui
- Todo o conteúdo do manual: preparo da palestra, benefícios, branding, plano B, checklist, FAQ etc.
- Login por e-mail: a pessoa digita o e-mail da inscrição e o site já preenche
  o painel com a palestra, trilha, horário, duração e formato dela, usando os
  dados da grade oficial (26 palestrantes com e-mail cadastrado no momento da geração).
- Os e-mails não ficam em texto puro no código — são comparados por hash, não
  é um mecanismo de segurança forte, apenas evita exposição trivial no "ver código-fonte".

## Como publicar com GitHub Pages
1. Suba este repositório para o GitHub (veja comandos abaixo).
2. Em *Settings → Pages*, escolha a branch `main` e a pasta `/ (root)`.
3. O GitHub vai gerar uma URL tipo `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Atualizar dados de palestrantes
A lista fica no `<script>` do próprio `index.html`, na constante `SPEAKERS`.
Sempre que a grade oficial mudar (novas pessoas, e-mails, horários), é só pedir
para eu regenerar esse bloco a partir de um CSV atualizado.
