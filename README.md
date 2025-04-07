# Ask-Adam 🕎

Sistema inteligente para criar estudos da religião judaica — com base na Torah, Tanakh e outros textos rabínicos — de forma respeitosa, profunda e fundamentada na tradição.

---

## 📦 Instalação

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/ask-adam.git
cd ask-adam
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

> Obs: Certifique-se de ter o [Ollama](https://ollama.com/) instalado e o modelo `llama3` já carregado localmente.

3. Execute o app:
```bash
streamlit run main.py
```

4. Acesse no navegador:
```
http://localhost:8501
```

---

## ✨ Funcionalidades

- **Geração de estudos judaicos indutivos** via IA com base em temas ou perguntas.
- **Upload de PDFs** com textos para análise automatizada.
- **Resposta formatada** com explicação, 10 perguntas (observação, interpretação e aplicação) e versículo final.
- **Salvamento automático** em `.txt`, `.md` e `.pdf` dos estudos gerados.
- **Interface com visual refinado**, inspirada em materiais de estudo judaico.

---

## 📁 Estrutura de Diretórios

```
ask-adam/
│
├── main.py                  # Interface principal Streamlit
├── .env                    # Arquivo de configuração de ambiente
├── requirements.txt        # Dependências
├── README.md               # Este arquivo ✨
│
├── estudos_salvos/         # Pasta onde os estudos são salvos automaticamente
│
└── src/                    # Código-fonte do agente
    ├── EBIagent.py         # Núcleo do agente de IA
    ├── gerador_pdf.py      # Função de exportação para PDF
    ├── textos.py           # Utilitários para gerar e formatar estudos
    └── styles.py           # Estilos e visuais customizados
```

---

## 🔧 Personalização

Você pode alterar os parâmetros do agente em `main.py`, como:
- Versão da Bíblia (Ex: Tanakh, Torah, etc)
- Público-alvo (Ex: judeus religiosos modernos, estudiosos etc)
- Linguagem (formal, simples, etc)

Exemplo:
```python
params = {
    "versao_biblia": "Tanakh (Judaico)",
    "publico": "judeus religiosos modernos",
    "linguagem": "formal e respeitosa",
    "base_fe": "judaica tradicional"
}
```

---

## 🤝 Contribuição

Sinta-se à vontade para abrir issues, enviar pull requests ou compartilhar com sua comunidade judaica local! Este projeto visa fortalecer o estudo da Torá com tecnologia acessível e ética.

---

## 📜 Licença

Este projeto está sob a Licença MIT.

---

Feito com 🕯️ por Willian Albarello e contribuições da comunidade.
