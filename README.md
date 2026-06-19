# 🚴 Renan Bike

Sistema web desenvolvido em **Flutter (Web)** utilizando **GetX** para gerenciamento de uma oficina mecânica de bicicletas.

---

## 📌 Visão Geral

O sistema permite o controle completo de clientes, serviços e manutenção recorrente, além de disponibilizar uma área pública com informações da loja.

---

## 🔐 Área Administrativa

- Login com autenticação
- Cadastro de clientes
- Registro de serviços:
  - Manutenção
  - Instalação de tubeless
  - Reparo de pneus
- Definição de prazo de retorno
- Alerta visual de retorno vencido
- Botão para contato via WhatsApp com mensagem automática

---

## 🌐 Área Pública

- Tabela de preços
- Descrição dos serviços
- Produtos da loja (capacetes, pneus, acessórios)

---

## 💬 Integração com WhatsApp

Ao expirar o prazo de retorno:
- Exibe botão automático
- Abre conversa no WhatsApp
- Mensagem pré-preenchida

---

## 🧱 Arquitetura (GetX)

```
lib/
├── app/
│   ├── bindings/        # Injeção de dependências
│   ├── controllers/     # Lógica (GetxController)
│   ├── data/
│   │   ├── models/
│   │   ├── providers/
│   │   ├── repositories/
│   ├── modules/         # Feature-first
│   │   ├── auth/
│   │   │   ├── views/
│   │   │   ├── controllers/
│   │   │   ├── bindings/
│   │   ├── clients/
│   │   ├── services/
│   │   ├── dashboard/
│   │   ├── public/
│   ├── routes/
│   │   ├── app_pages.dart
│   │   ├── app_routes.dart
│   ├── core/
│   │   ├── theme/
│   │   ├── utils/
│   │   ├── constants/
│   ├── widgets/
│
├── main.dart
```

---

## 🎨 Identidade Visual

Baseada no logotipo (preto + amarelo metálico + cinza):

- **Primary:** `#F2C94C` (Amarelo destaque)
- **Secondary:** `#1C1C1C` (Preto profundo)
- **Tertiary:** `#BDBDBD` (Cinza metálico)
- **Error:** `#EB5757` (Vermelho alerta)
- **Neutral:** `#2F2F2F`
- **Neutral Variant:** `#828282`

---

## 🚀 Como rodar

```bash
flutter pub get
flutter run -d chrome
```

---

## 📈 Futuras melhorias

- Dashboard com métricas
- Notificações automáticas
- Histórico do cliente
- Agenda de serviços
- Multi-usuários

---

## 📄 Licença

MIT
