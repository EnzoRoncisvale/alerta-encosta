# Guia de Gravação e Roteiro Oficial do Pitch (Até 5 Minutos)

**Projeto:** AlertaEncosta  
**Disciplina:** H3-AC — Arquiteturas Convergentes — Sistematização (CEUB)  
**Critério no Edital:** Item 11 — Pitch (Vídeo de até 5 minutos) | Pontuação: 0,5 ponto  

---

## 🛠️ Como Gravar o Vídeo em Menos de 10 Minutos (Sem Instalar Programas Complexos)

Você tem à disposição duas ferramentas fáceis e gratuitas:

### Opção 1: Barra de Jogos do Windows (Nativa — Win + Alt + R)
1. Abra o arquivo `apresentacao_slides.html` no Google Chrome ou Edge.
2. Pressione **F11** para colocar os slides em tela cheia.
3. Pressione o atalho do Windows: **`Win + Alt + R`** (ou abra a Game Bar com `Win + G` e clique em gravar). Certifique-se de que o microfone esteja ativado.
4. Fale o roteiro lendo as notas de cada slide (use as setas para avançar os slides).
5. Ao terminar, pressione **`Win + Alt + R`** novamente. O vídeo fica salvo em `Vídeos\Capturas`.

### Opção 2: Clipchamp / Loom / OBS / PowerPoint
- No PowerPoint: clique em **Gravar > Gravação de Tela**.
- No Clipchamp (nativo do Windows 11): **Gravar tela e câmera**.
- No Loom ou OBS: selecione a janela do navegador.

---

## ⏱️ Roteiro Palavra por Palavra com Marcação de Tempo

*Tempo total estimado: 4 minutos e 15 segundos (folga confortável dentro do limite de 5 minutos).*

---

### [0:00 - 0:25] Abertura e Identificação
*(Exibir o **Slide 1** — Capa)*

> "Olá, professor e avaliadores. Meu nome é **Enzo Roncisvale**, estudante de Ciência da Computação / Engenharia de Software no CEUB.  
> Apresento a sistematização da disciplina Arquiteturas Convergentes: o projeto **AlertaEncosta**, uma proposta computacional voltada à integração de dados ambientais e ao apoio ao registro padronizado de alertas de Defesa Civil em áreas de encosta, alinhada diretamente ao Plano Nacional de Proteção e Defesa Civil (o PN-PDC 2025–2035)."

---

### [0:25 - 1:10] Pergunta 1: Qual é o problema?
*(Avançar para o **Slide 2** — O Problema)*

> "Passando para a primeira pergunta: **Qual é o problema?**  
> No Brasil, desastres causados por escorregamentos de terra em encostas urbanas provocam mortes e perdas irreparáveis todos os anos.  
> Do ponto de vista técnico e computacional, o gargalo das Defesas Civis municipais é a **dispersão dos dados de monitoramento**. Os pluviômetros, dados do Cemaden e sensores de solo operam em sistemas isolados.  
> Durante temporais extremos, o agente de plantão precisa consultar várias janelas, calcular limiares manualmente e redigir alertas sem apoio integrado. Essa sobrecarga cognitiva gera atrasos perigosos no instante em que cada minuto ganho é vital para salvar vidas."

---

### [1:10 - 1:55] Pergunta 2: Qual meta do PN-PDC está sendo trabalhada?
*(Avançar para o **Slide 3** — Meta do PN-PDC)*

> "Segunda pergunta: **Qual meta do PN-PDC está sendo trabalhada?**  
> Nosso projeto atua formalmente na **Meta 2.2.2** do PN-PDC 2025–2035, instituído pelo Decreto Federal nº 12.652/2025 e regulamentado pela Portaria MIDR nº 3.318/2025.  
> A descrição oficial da Meta 2.2.2 é:  
> *'Elaborar e atualizar protocolo conjunto de monitoramento e envio de alertas de modo a unificar esses procedimentos'*.  
> Essa meta está vinculada ao **Objetivo 2.2**, que visa expandir e aperfeiçoar os sistemas de monitoramento e alerta, dentro do eixo de **Preparação**. O prazo pactuado para o seu marco inicial é de **curto prazo, até 2027**, com revisões contínuas ao longo do plano."

---

### [1:55 - 2:45] Pergunta 3: Como a Computação contribui para atingir essa meta?
*(Avançar para o **Slide 4** — Papel da Computação)*

> "Terceira pergunta: **Como a Computação contribui para atingir essa meta?**  
> A Ciência da Computação viabiliza essa unificação através de uma **arquitetura convergente**, unindo IoT virtual, processamento de regras determinísticas e interfaces web reativas.  
> O sistema ingere os dados telemétricos, descarta anomalias, detecta perda de sinal telemétrico (classificando dados com mais de 30 segundos como desatualizados) e pré-avalia os limiares operacionais.  
> Importante ressaltar: a computação aqui adota o princípio *Human-in-the-Loop*. Ela não dispara alarmes sozinha: ela elimina o trabalho mecânico e entrega ao analista humano os dados já triados, com uma minuta padronizada no padrão internacional CAP e registro de auditoria imutável."

---

### [2:45 - 3:50] Pergunta 4: Como a solução funciona?
*(Avançar para o **Slide 5** — Funcionamento da Solução)*

> "Quarta pergunta: **Como a solução funciona?**  
> O AlertaEncosta opera em três camadas claras:  
> **1. Entrada:** recebe leituras de chuva acumulada de 1 hora e saturação volumétrica do solo em três setores da comunidade fictícia: Vila Alta, Morro da Esperança e Encosta Sul.  
> **2. Processamento:** aplica um filtro de validação física e avalia a regra combinada didática: chuva em 1 hora maior ou igual a 30 milímetros E umidade do solo maior ou igual a 80%. Ao atingir essa condição, o evento é colocado na fila prioritária de triagem.  
> **3. Saída:** apresenta um painel de comando intuitivo, sinaliza visualmente a encosta em risco e abre um formulário de decisão padronizada. Para registrar o despacho, o operador deve obrigatoriamente assinar com seu identificador e redigir uma justificativa técnica de no mínimo 15 caracteres, gerando o arquivo JSON auditável."

---

### [3:50 - 4:40] Pergunta 5: Como será medido o resultado?
*(Avançar para o **Slide 6** — Indicador de Resultado)*

> "Quinta e última pergunta: **Como será medido o resultado?**  
> Definimos um indicador quantitativo e mensurável: a **Redução Percentual do Tempo Médio de Análise e Despacho de Alerta**, expressa pela fórmula:  
> `Redução (%) = [(Tm - Ta) / Tm] * 100`,  
> onde *Tm* é o tempo do fluxo manual descentralizado e *Ta* é o tempo do fluxo apoiado pelo AlertaEncosta.  
> Estabelecemos uma meta de reduzir pelo menos 30% do tempo.  
> Em nossos ensaios experimentais cronometrados, o tempo médio manual foi de 48,7 segundos, enquanto no fluxo convergente caiu para 26,3 segundos. Isso representou uma **redução de 46% no tempo de despacho**, garantindo 100% de completude nos registros de auditoria."

---

### [4:40 - 5:00] Fechamento e Conclusão
*(Avançar para o **Slide 7** — Conclusão)*

> "Em conclusão, o AlertaEncosta comprova que a computação convergente pode transformar uma exigência estratégica do PN-PDC em uma ferramenta operacional real, ágil e segura, preservando sempre o protagonismo humano na gestão de desastres.  
> O protótipo interativo e toda a documentação estão disponíveis no pacote entregue.  
> Muito obrigado pela atenção!"

---

## 🎯 Dicas para tirar Nota Máxima no Pitch (0,5 ponto)
1. **Fale com clareza e segurança:** siga o roteiro sem pressa; você terá quase 1 minuto de sobra.
2. **Mostre os slides ou o protótipo:** enquanto fala sobre o funcionamento, você pode até alternar por 15 segundos para a janela do protótipo `index.html` e demonstrar um clique no botão "Crítico no Setor B".
3. **Verifique o áudio:** antes de gravar o vídeo inteiro, faça um teste de 10 segundos para ver se o microfone está captando com bom volume.
