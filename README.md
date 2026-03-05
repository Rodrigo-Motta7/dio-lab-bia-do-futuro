# 🎓 Digo — Educador Financeiro com IA Generativa

> *"Eae, me chamo Digo. Como posso te ajudar sobre finanças?"*

Digo é um agente de IA generativa criado para **educar iniciantes em finanças pessoais**, explicando conceitos como tipos de investimento, reserva de emergência e planejamento financeiro — de forma simples, acessível e sem jargão.

---

## 🧠 O que o Digo faz

- Explica conceitos financeiros básicos sob demanda
- Responde dúvidas sobre investimentos, reservas e finanças pessoais
- Age como um professor particular: informal, próximo e didático
- Cita a fonte das informações para evitar alucinações

## 🚫 O que o Digo **não** faz

- Não recomenda investimentos específicos
- Não vaza dados bancários do usuário
- Não responde fora do escopo financeiro-educacional

---

## 🗂️ Estrutura do Repositório

```
📁 dio-lab-bia-do-futuro/
├── 📁 data/
│   ├── transacoes.csv
│   ├── historico_atendimento.csv
│   ├── perfil_investidor.json
│   └── produtos_financeiros.json
├── 📁 docs/
│   ├── 01-documentacao-agente.md
│   ├── 02-base-conhecimento.md
│   ├── 03-prompts.md
│   ├── 04-metricas.md
│   └── 05-pitch.md
├── 📁 src/
│   └── app.py
└── README.md
```

---

## ⚙️ Stack

| Componente | Tecnologia |
|---|---|
| LLM | Ollama (modelo local) |
| Interface | Chatbot via terminal / app |
| Base de conhecimento | JSON + CSV mockados |
| Validação | Checagem de fontes + limitações declaradas |

---

## 🛡️ Segurança e Anti-Alucinação

- Respostas baseadas apenas nos dados fornecidos
- Toda resposta cita a fonte utilizada
- Quando não sabe, o Digo declara a limitação abertamente
- Dados bancários nunca são expostos

---

## 🚀 Como Rodar

```bash
# Clone o repositório
git clone https://github.com/Rodrigo-Motta7/dio-lab-bia-do-futuro.git
cd dio-lab-bia-do-futuro

# Instale as dependências
pip install -r requirements.txt

# Inicie o Ollama localmente
ollama serve

# Execute o agente
python src/app.py
```

---

## 👤 Persona

**Nome:** Digo  
**Tom:** Informal e educativo — como um professor particular  
**Público-alvo:** Iniciantes no mundo dos investimentos  

| Situação | Exemplo |
|---|---|
| Saudação | *"Eae, me chamo Digo. Como posso te ajudar sobre finanças?"* |
| Confirmação | *"Ok, vou dar uma olhada e já retorno."* |
| Limitação | *"Não consigo te ajudar com isso no momento."* |

---

## 📄 Documentação

A documentação completa do agente está na pasta [`docs/`](./docs/), cobrindo arquitetura, prompts, base de conhecimento, métricas e pitch.

---

*Desenvolvido como parte do lab DIO — Agente Financeiro com IA Generativa.*
