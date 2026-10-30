# Landing page PJR: guia de publicação

Arquivo principal: `index.html` (HTML + CSS + JS em um só arquivo, sem build).
Pasta `assets/` com imagens, logos, favicon e imagem de compartilhamento.

## Antes de publicar (obrigatório)
1. **Domínio:** hoje o endereço é o do GitHub Pages (`https://samubhz.github.io/pjr-consultoria-tributaria/`). Ao ligar um domínio próprio, troque-o em `index.html` (canonical, Open Graph, JSON-LD), `robots.txt` e `sitemap.xml`.
2. **Formulário:** em `index.html`, procure `FORM_ENDPOINT` e coloque a URL de um serviço (Formspree, Make, Zapier, Formspark etc.). Enquanto estiver vazio, o envio abre o e-mail do visitante com a mensagem preenchida.
3. **Contatos:** confira e-mail e telefone (hoje: reinaldo@pauloteodoro.adv.br e (31) 98722-8207; o e-mail ainda usa o domínio do escritório antigo).
4. **OAB:** submeta o texto à Comissão de Publicidade/Ética da OAB seccional (ou ao responsável do escritório) antes de ir ao ar.
5. **Política de privacidade:** o formulário cita a LGPD; publique uma página de política de privacidade e linke no rodapé.
6. **Datas e normas:** o conteúdo reflete a legislação conhecida até outubro de 2026. Revise o texto a cada atualização da regulamentação.

## SEO já incluído
- `<title>` e meta description otimizados, canonical, robots, theme-color.
- Open Graph e Twitter Card (imagem 1200x630 em `assets/og-image.jpg`).
- Dados estruturados (JSON-LD): WebSite, LegalService/ProfessionalService, Person e FAQPage (gerado das mesmas perguntas visíveis na página).
- Hierarquia H1 > H2 > H3, HTML semântico, `alt` em todas as imagens, links âncora.
- Imagens com tamanho declarado, `loading="lazy"` e preload da imagem principal (assets/biblioteca.jpg).
- `robots.txt` e `sitemap.xml`.

## Depois de publicar
- Cadastre o site no **Google Search Console** e envie o `sitemap.xml`.
- Crie/reivindique o perfil no **Google Meu Negócio** (se houver endereço) e aponte para a página.
- Instale um medidor (Google Analytics 4 ou Plausible). Se usar cookies, adicione aviso de cookies (LGPD).
- Teste em https://pagespeed.web.dev e em https://search.google.com/test/rich-results.
- Para crescer em buscas: crie páginas/artigos por tema (ex.: "split payment no transporte", "reforma tributária na construção civil") linkando para esta página.

## Observações de conformidade (OAB)
A página foi escrita sem preço, sem "grátis", sem promessa de resultado e sem chamadas de captação; o contato é espontâneo. O checklist é material educativo de autoavaliação. Mantenha esse padrão ao editar.

## Animações
- Entradas suaves ao rolar (fade + deslocamento curto, com escalonamento de até 50 ms por item).
- Topo com entrada em sequência; fotos com revelação por máscara; linha do cronograma que se desenha; zoom lento na faixa da citação.
- Botões com feedback ao clique; cartões com elevação no hover (apenas em dispositivos com mouse).
- Checklist: marca de seleção animada e anel de progresso que preenche suavemente.
- FAQ abre e fecha com transição de altura (Chrome/Edge/Safari recentes; nos demais, abre sem animação).
- Cabeçalho ganha sombra ao rolar e o botão do WhatsApp aparece depois de rolar a página.
- Só `transform` e `opacity` são animados. Para quem ativa "reduzir movimento" no sistema, nenhuma animação roda e o conteúdo aparece direto. Sem JavaScript, o conteúdo também aparece normalmente.

## Auditoria de SEO (30/10/2026)
Aplicado: título (50 car.) e descrição (151 car.) dentro do limite; palavra-chave "Reforma Tributária" no H1; glossário com 8 termos (+ DefinedTermSet); FAQPage, WebPage e catálogo de serviços no JSON-LD; hreflang; fonte carregada sem bloquear a renderização; imagens em WebP (de 2,0 MB para 1,2 MB); páginas `privacidade.html` e `404.html`; sitemap com lastmod.
Ainda depende de você: endereço e CNPJ/razão social (para dados locais e Google Meu Negócio), domínio próprio, Search Console e artigos de blog (ver recomendações).

## Artigos (blog)
Pasta `artigos/` com a listagem e 6 artigos (split payment, cClassTrib, construção civil e contratos, créditos de PIS e Cofins, transporte de cargas e apuração assistida). Estilo em `assets/blog.css`. Para criar novos artigos, copie um arquivo existente, troque título, descrição, `canonical`, conteúdo e o JSON-LD, e acrescente a URL em `sitemap.xml` e o cartão na home. Mantenha o tom informativo (sem preço, promessa de resultado ou chamadas de captação) e revise na OAB.
