# Nossa Viagem a Miami — primeira versão

Site estático, responsivo e mobile-first para o roteiro de 18/11/2026.

## Testar localmente
1. Extraia o ZIP.
2. Abra `index.html` no navegador. Para melhor compatibilidade, use uma extensão de servidor local ou execute `python3 -m http.server 8000` na pasta e abra `http://localhost:8000`.

## Publicar na Vercel (sem terminal)
1. Acesse https://vercel.com/ e entre/crie uma conta.
2. Crie um repositório no GitHub e envie `index.html` para a raiz do repositório.
3. Na Vercel, selecione **Add New → Project** e importe o repositório.
4. Como é um site estático, não precisa de framework nem build command. Se a Vercel pedir, deixe Build Command vazio e Output Directory como `.`.
5. Clique em **Deploy**. A Vercel fornecerá um endereço `*.vercel.app` que você pode compartilhar com sua namorada.

## Publicar sem GitHub
Na Vercel, use a opção de deploy pela CLI se você já tiver Node.js instalado:
- `npm i -g vercel`
- entre na pasta que contém `index.html`
- execute `vercel`
- siga as perguntas e depois execute `vercel --prod` para publicar a versão de produção.

## O que funciona
- Layout adaptado para celular e desktop.
- Botões de navegação do Google Maps para cada trecho e para o percurso completo.
- Mapa incorporado da região de Miami.
- Checkboxes de progresso salvos no navegador atual.

## Limitações desta versão
- As marcações ficam salvas apenas no navegador/dispositivo usado; não sincronizam entre duas pessoas.
- O mapa incorporado mostra a região de Miami, enquanto o botão abre a rota com as paradas no Google Maps.
- Fotos e fontes são carregadas de serviços externos; é necessária conexão à internet.
- Confirme endereços, funcionamento, tarifas e trânsito perto da viagem. Horários do roteiro são estimativas.
