meu-projeto/
├── run.py                 # Arquivo que inicia o servidor
├── app/                   # Pasta principal do código
│   ├── __init__.py        # Transforma a pasta em um pacote
│   ├── routes/            # Sub-pastas para organizar as rotas
│   │   ├── auth.py        # Login/Cadastro (Supabase)
│   │   ├── payments.py    # Integração Mercado Pago
│   │   └── views.py       # Renderiza seus HTMLs
│   ├── static/            # Seus CSS, JS e Imagens
│   └── templates/         # Seus arquivos HTML (organizados)
│       ├── base.html
│       ├── auth/          # HTMLs de login
│       └── shop/          # HTMLs da loja
├── requirements.txt       
└── .env