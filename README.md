# AlertaEncosta — Pacote de Entrega Oficial

**Disciplina:** H3-AC — Arquiteturas Convergentes — Sistematização  
**Instituição:** CEUB (Centro Universitário de Brasília)  
**Projeto:** AlertaEncosta: Arquitetura Convergente para Integração de Dados Ambientais e Apoio ao Registro Padronizado de Alertas em Áreas de Encosta  
**Vinculação ao PN-PDC 2025–2035:** Meta 2.2.2 (Decreto Federal nº 12.652/2025 e Portaria MIDR nº 3.318/2025)  

---

## 📁 Estrutura de Arquivos do Pacote

1. **`index.html`** — **Protótipo Interativo Funcional**:
   - Single-Page Application (SPA) em HTML5/CSS3/JavaScript puro (sem dependências externas de internet).
   - Painel de comando de Defesa Civil com 3 setores telemétricos (Vila Alta, Morro da Esperança, Encosta Sul).
   - Injeção dinâmica de cenários pré-configurados e teste paramétrico.
   - Detecção automática de dados desatualizados (> 30s) e sanitização de entradas inválidas.
   - Módulo de protocolo unificado (Meta 2.2.2) com decisão humana obrigatória (*Human-in-the-Loop*).
   - Laboratório experimental cronometrado para medição em tempo real de $T_m$, $T_a$ e % de redução de tempo.
   - Histórico auditável gravado em `localStorage` e exportador de dados JSON (formato CAP).

2. **`relatorio_tecnico.html`** — **Relatório Técnico Acadêmico Completo**:
   - Atende aos 17 itens obrigatórios do edital com diagramas SVG de alta resolução.
   - Otimizado para leitura na tela e para impressão/salvamento em PDF (`Ctrl + P` ou botão nativo "Imprimir").
   - Contém matriz completa de critérios de avaliação (10,0 pontos) e referências bibliográficas oficiais.

3. **`RELATORIO_TECNICO.md`** — **Relatório Técnico em Formato Markdown**:
   - Versão padrão Markdown para consulta e documentação versionada.

4. **`apresentacao_slides.html`** — **Pitch Deck Interativo (Slides de Apresentação)**:
   - Apresentação visual em tela cheia com navegação por teclado (setas ◀ / ▶ ou barra de espaço).
   - Responde diretamente às 5 perguntas obrigatórias do Pitch do edital.
   - Inclui botão de "Notas do Orador" contendo o roteiro de fala para cada slide.

5. **`ROTEIRO_PITCH_5_MINUTOS.md`** — **Roteiro e Guia de Gravação do Pitch**:
   - Script palavra por palavra com marcação de tempo (total de 4m15s).
   - Instruções práticas para gravação rápida da tela usando o Windows (`Win + Alt + R`), Clipchamp, OBS ou Loom.

6. **`AlertaEncosta_Entrega_Final.zip`** — **Arquivo ZIP Consolidado para Submissão no Moodle**:
   - Pacote único compactado conforme a exigência da Seção 10 do edital.

---

## 🚀 Como Executar e Testar o Protótipo

1. Dê um duplo clique no arquivo **`index.html`** (ele abrirá diretamente no Google Chrome, Microsoft Edge ou Firefox).
2. Não é necessário instalar Node.js, Python ou bibliotecas extras: o protótipo funciona 100% offline.
3. Para testar o acionamento de alerta:
   - Clique no botão **"🔴 2. Crítico no Setor B"** no menu lateral.
   - Veja o setor Morro da Esperança atingir a condição de alarme e entrar na fila de triagem.
   - Clique na aba **"📝 Protocolo Padronizado"**, preencha os dados e salve a decisão.
   - Consulte o registro gravado na aba **"📜 Histórico & Auditoria"** e teste o botão de exportar JSON.
4. Para testar o indicador cronometrado ($T_m$ vs. $T_a$):
   - Abra a aba **"⏱️ Ensaio Experimental"**, selecione o fluxo e clique em **"Iniciar Ensaio"**.

---

## 📋 Checklist Antes de Entregar no Moodle do CEUB

- [ ] Abrir `relatorio_tecnico.html` ou `RELATORIO_TECNICO.md` e preencher seu **Nome Completo** e **Matrícula**.
- [ ] (Opcional, para garantir o 0,5 ponto do Pitch): Abrir `apresentacao_slides.html`, gravar a tela lendo o roteiro de `ROTEIRO_PITCH_5_MINUTOS.md` (leva 4 minutos) e colocar o arquivo de vídeo gerado (`video_pitch.mp4`) dentro do ZIP.
- [ ] Submeter o arquivo **`AlertaEncosta_Entrega_Final.zip`** na página da tarefa:  
  `https://campusonline2.ceub.br/mod/assign/view.php?id=14735`
