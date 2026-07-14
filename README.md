# Como seus clientes usam e pagam

## 🧑‍💻 Como usam

```
1. Abrem https://root.eternets no celular/PC
2. Geram chave (1 clique, zero cadastro) ← JÁ FUNCIONA
3. Usam os serviços:
   ├── 💳 FreePay → transferir CTF entre si
   ├── 🔐 VOID License → gerar licença
   └── 🛡️ PQC Shield → enviar lead
```

## 💰 Como te pagam

Sem banco, sem Stripe, sem PayPal. Tudo em **Bitcoin Lightning**.

### FreePay (CTF)
```
Cliente adquire CTF → usa FreePay → você recebe CTF
└── CTF pode ser trocado por BTC via swap P2P
```
*Lucro:* Taxa 0% (usa CTF como utilitário, não como especulação)

### VOID License — $500 a $50.000
```
Cliente vê preço em USD → paga em BTC/Lightning → você gera licença
```

### PQC Shield — $5.000 a $100.000
```
Cliente envia lead via Nostr → você propõe → fecha via contrato inteligente
                                        ↓
                                Pagamento em BTC/Lightning
```

## ⚡ Lightning = zero banco

| Vantagem | BTC/Lightning | Cartão/Boleto |
|---|---|---|
| Conta bancária | ❌ não precisa | ✅ precisa |
| Taxa | ~0.1% | 2-5% |
| Chargeback | ❌ impossível | ✅ vulnerável |
| Internacional | ✅ automático | ✅ complexo |
| Anônimo | ✅ opcional | ❌ KYC |

## Receber pagamentos (3 formas)

### 1. Lightning Address (mais fácil)
```
Cria em: https://getalby.com  ou  https://ln.tips
Exemplo: pagamentos@eternets.com
Cliente paga de qualquer wallet Lightning
Custo: $0
```

### 2. LNURL-pay (widget no site)
```
QR Code fixo que cliente escaneia e paga
Pode gerar invoices dinâmicas via API
Custo: $0 (OpenNode ou LNbits)
```

### 3. On-chain BTC (grandes valores)
```
Para vendas > $1.000 — cliente envia BTC on-chain
Taxa: ~$0.50 a $5 (independente do valor)
```

## Fluxo prático de venda

```
1. Cliente acessa root → aba License → escolhe plano
2. Vê: "VOID Pro — $5.000 | Pay with Lightning"
3. Clica → vê QR Code da invoice
4. Paga com Phoenix/Breez/WoS
5. Você recebe BTC na hora (confirmação em 1-3s)
6. Abre root → gera licença → publica evento Nostr
7. Cliente verifica: curl https://root.eternets/api/license/verify/ID
```

## O que precisa fazer agora

```
1️⃣ Criar Lightning Address em getalby.com (2 minutos, grátis)
2️⃣ Copiar o LNURL para colocar no root.html
3️⃣ Pronto — pode vender
```
