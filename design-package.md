# Design Package: COOPE

## 1. Premissa da Marca
No agronegócio, quem caminha sozinho arca com todos os riscos de mercado e de clima. A Coope une a força de milhares de produtores para negociar insumos pelo menor custo, garantir a armazenagem e o escoamento total da colheita e devolver o resultado diretamente para quem trabalha a terra de Pernambuco.

## 2. Paleta de Cores (Tokens CSS)
```css
:root {
  --canvas: #0D150F;
  --panel: #162319;
  --panel-light: #1E3022;
  --accent: #E2A838;
  --accent-hover: #F0B84D;
  --accent-muted: rgba(226, 168, 56, 0.18);
  --text-primary: #F2F6F3;
  --text-secondary: #9EB4A2;
  --border: rgba(158, 180, 162, 0.18);
  --border-focus: #E2A838;
}
```

## 3. Trio Tipográfico
- Display: Fraunces (600, 700)
- Corpo: Plus Jakarta Sans (400, 500, 600)
- Dados e Métricas: Space Mono (400, 700)

## 4. Mapa de Faixas do Hero (Band Map)
| Faixa | Intervalo | Momento da Imagem | Texto Exato | Entrada |
|---|---|---|---|---|
| 1 | 0.00 a 0.20 | Vista aérea da lavoura ao amanhecer | "A terra produz. A união prospera." | Rise settle no carregamento |
| 2 | 0.24 a 0.46 | Descida suave sobre a plantação madura | "Insumos com poder de compra coletivo. O custo certo na hora do plantio." | Drift-down |
| 3 | 0.50 a 0.72 | Aproximação dos silos e estruturas | "Armazenagem segura e agrônomos ao seu lado dentro da porteira." | Grid snap-align |
| 4 | 0.76 a 1.00 | Enquadramento estável da sede e da colheita | "Coope. O resultado da safra valorizado em cada hectare." | Staged settle com botão |

## 5. Hero Estático (Mobile e Movimento Reduzido)
- Título: "A terra produz. A união prospera."
- Subtítulo: "Segurança de armazenagem, compra conjunta de insumos e retorno proporcional de sobras para o produtor rural."
- Botão: "Associe-se à Coope"

## 6. Estrutura Abaixo do Hero
1. Barra de Indicadores de Confiança: 3.200 cooperados, 1.4 milhão de sacas armazenadas, R$ 42 milhões em sobras distribuídas, 38 anos de solidez.
2. Pilares de Apoio ao Cooperado:
   - Compra Coletiva de Insumos: fertilizantes e defensivos com preço negociado em grande escala.
   - Assistência Técnica no Campo: agrônomos dedicados que visitam a propriedade.
   - Armazenagem e Logística: silos modernos para guardar a produção sem filas ou perdas.
   - Comercialização e Exportação: acesso direto aos mercados e tradings globais.
3. Momento Interativo:
   - Simulador de Benefício do Cooperado: o visitante seleciona a área plantada (em hectares) e o simulador calcula a economia média em insumos e a estimativa de sobras da safra.
4. Voz do Cooperado:
   - Depoimentos reais e fotos de produtores agrícolas de Pernambuco.
5. Perguntas Frequentes (FAQ):
   - Como funciona a divisão de sobras ao fim do ano?
   - Pequenos produtores recebem a mesma atenção técnica que grandes fazendas?
   - Quais são os requisitos para se associar à cooperativa?
   - Como entrego e armazeno a minha produção?
6. Formulário de Associação:
   - Campos: Nome completo, Telefone/WhatsApp, Município e Estado, Área da propriedade (ha), Cultura principal.
   - Botão de envio: "Solicitar contato de um agrônomo".
   - Feedback: mensagem de confirmação com retorno previsto em até 24 horas.
7. Rodapé Institucional:
   - Dados de contato, ouvidoria, selo de cooperativismo e nota declarando a Coope como cooperativa modelo institucional de Pernambuco.

## 7. Camada de Vetores (SVG)
- Linhas suaves de curvas de nível topográficas que se desenham conforme a rolagem.
- Partículas sutis no fundo simulando poeira dourada ao pôr do sol na lavoura.

## 8. Padrão de Engenharia
- Carregamento de vídeo via Blob com anel de progresso SVG.
- Suavização lerp normalizada para 60fps no requestAnimationFrame.
- Seek com bloqueio anti-deadlock.
- Escritas no DOM disparadas apenas quando há alteração real.
- Suporte total a telas pequenas e prefers-reduced-motion.

## 9. Regra de Revisão de Texto
- Proibição de travessões (em dashes).
- Proibição de palavras corporativas genéricas. Linguagem direta, clara e humana.
