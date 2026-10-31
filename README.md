# AccessHub Demo

Demonstração web independente de gestão associativa e identificação digital, idealizada por Rubens Eduardo.

**Atenção:** este projeto é uma demonstração. Todos os registros são fictícios. Não é o sistema operacional finalizado da ADEMOC, não contém dados reais da associação e não deve ser utilizado para identificação oficial. Todas as logomarcas e tags de identificação foram removidas. 

## Funcionalidades
- Dashboard com indicadores calculados a partir dos registros locais.
- Cadastro de associados fictícios com numeração única `AH-2026-XXXX`.
- Pesquisa e filtro por situação.
- Exportação CSV dos dados de demonstração.
- Carteirinha demonstrativa com QR Code.
- Consulta/validação local do número de identificação.
- Controles básicos de acessibilidade: tamanho de fonte, alto contraste e link para pular ao conteúdo.
- Persistência local no navegador via `localStorage`.

## Publicar no GitHub Pages
1. Crie um repositório público chamado `accesshub-demo` (ou outro nome).
2. Envie o conteúdo desta pasta diretamente para a raiz do repositório.
3. Em **Settings → Pages**, selecione **Deploy from a branch**, branch `main`, pasta `/ (root)`.
4. Aguarde a publicação.

## Executar localmente
Abra `index.html` em um navegador. O QR Code utiliza a biblioteca QRCode.js via CDN; sem conexão, o restante da demonstração funciona e o QR Code pode não ser exibido.

## Limitações e segurança
- `localStorage` é apenas armazenamento local, não é banco de dados multiusuário.
- Não há autenticação, autorização, criptografia de dados em trânsito ou servidor.
- A validação é apenas uma consulta à base local e pode ser alterada pelo próprio usuário.
- Não inserir dados pessoais reais ou informações de associados.
- Para uma implantação real, será necessário backend seguro, controle de acesso, auditoria, política de retenção, avaliação de impacto à proteção de dados e revisão de acessibilidade.

## Contexto do projeto
O projeto original foi implementado com planilhas e banco de dados local para apoiar cadastro, controle, numeração única, emissão e consulta de carteirinhas. Esta versão web é uma reconstrução demonstrativa e independente, não uma cópia do sistema original.
