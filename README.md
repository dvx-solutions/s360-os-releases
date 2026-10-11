# S360-OS — downloads

Instaladores do **S360-OS**, o app desktop com Agente de IA da Solução 360. O código-fonte é privado; este repositório só hospeda os instaladores.

Baixe a versão mais recente em **[Releases](../../releases/latest)**. Para entrar, use sua conta da Solução 360 (Tenant, e-mail e senha).

## Windows
`S360-OS-Setup-<versão>.exe`. O instalador ainda não é assinado: no aviso do SmartScreen, clique em **Mais informações → Executar assim mesmo**. Depois de instalado, o app se atualiza sozinho ("Reiniciar e atualizar").

## Linux (x64)
- `S360-OS-<versão>-linux-x86_64.AppImage` (recomendado): `chmod +x` e abra. Se atualiza sozinho.
- `S360-OS-<versão>-linux-x86_64.deb`: `sudo apt install ./S360-OS-<versão>-linux-x86_64.deb`. A atualização pelo app pede a senha de administrador; se falhar, baixe o `.deb` novo aqui.

Sem chaveiro do sistema (GNOME Keyring/KWallet), o login fica salvo sem criptografia forte. Em alguns ambientes (ex.: GNOME sem extensão de AppIndicator) o ícone da bandeja não aparece; abra o S360-OS de novo para trazer a janela.

## macOS
1. Baixe `S360-OS-<versão>-mac-arm64.dmg` (Apple M1/M2/M3/M4) ou `S360-OS-<versão>-mac-x64.dmg` (Intel). Em  › Sobre este Mac: "Chip Apple" = arm64, "Processador Intel" = x64.
2. Abra o .dmg e arraste o S360-OS para Aplicativos.
3. O app ainda não é assinado pela Apple, então o macOS bloqueia a primeira abertura. Libere de um destes jeitos:
   - Terminal: `xattr -dr com.apple.quarantine /Applications/S360-OS.app` e abra normalmente; ou
   - Tente abrir uma vez, vá em **Ajustes do Sistema › Privacidade e Segurança** e clique em **Abrir Mesmo Assim**.
4. Atualizações: o app avisa quando há versão nova; clique em **Baixar nova versão**, baixe o .dmg e substitua o app em Aplicativos (repita o passo 3).
