# Acesso de Emergência — Rede UFPI (CSHNB - Picos)

Página alternativa de emergência para login direto na rede da UFPI Picos, em caso de instabilidade na página original.

🔗 **Link de Acesso (GitHub Pages)**:
👉 **[https://gabreudev.github.io/auth-ufpi-page/](https://gabreudev.github.io/auth-ufpi-page/)**

---

## 🚀 Publicação no GitHub Pages

1. Inicialize e faça o push dos arquivos:
   ```bash
   git init
   git add .
   git commit -m "feat: login institucional ufpi picos"
   git branch -M main
   git remote add origin https://github.com/<seu-usuario>/<nome-do-repo>.git
   git push -u origin main
   ```
2. No GitHub:
   - Acesse **Settings** > **Pages**.
   - Em **Build and deployment**, selecione **Deploy from a branch**.
   - Escolha a branch `main` e a pasta `/(root)`.
   - Clique em **Save**.

---

## 🛠️ Especificações da Requisição

- **URL de Destino**:
  `https://login.picos.ufpi.br:6082/php/uid.php?vsys=1&rule=0`
- **Método**: `POST`
- **Encoding**: `application/x-www-form-urlencoded`
- **Campos**:
  - `user`: Usuário / Matrícula / CPF
  - `passwd`: Senha
  - `ok`: `Login`
  - `buttonClicked`: `0`
  - `redirect_url`: `https://www.globo.com`
  - `err_flag`: `0`
  - `inputStr`: `""`
  - `escapeUser`: `""`
  - `preauthid`: `""`
