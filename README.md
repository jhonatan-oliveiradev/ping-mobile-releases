# PING Mobile — Android Releases

Canal público de distribuição das builds Android do **PING**.

> **Beta técnica:** esta versão destina-se a testes. Mensagens E2EE, chamadas de voz/vídeo e notificações push ainda não estão disponíveis. Para conversar normalmente, utilize a versão web ou Desktop do PING.

## Instalar

1. Abra [Releases](https://github.com/jhonatan-oliveiradev/ping-mobile-releases/releases).
2. Escolha a versão beta publicada mais recente.
3. Em **Assets**, baixe o arquivo `.apk`.
4. No Android, abra o APK e, caso solicitado, permita a instalação pela fonte utilizada.
5. Confira a origem do download e mantenha o dispositivo atualizado.

**Atenção:** só haverá APK disponível depois que o mantenedor publicar uma release e anexar o binário. Este repositório **não** contém o código-fonte da aplicação.

## Primeira release planejada

- **Tag:** `android-v0.1.0-beta.1`
- **Título:** `PING Mobile 0.1.0-beta.1 — Android`
- **Arquivo:** `PING-Mobile-0.1.0-beta.1.apk`
- **Canal:** *Pre-release*
- **Origem:** build Android do EAS Expo, perfil `preview`

O nome da versão pode ser ajustado pelo mantenedor antes da publicação, mas a tag, o filename e a URL de download precisam permanecer coerentes.

## Integridade

Junto ao APK, publique um arquivo `SHA256SUMS.txt` com o hash SHA-256 do artefato efetivamente distribuído. Em Windows PowerShell:

```powershell
Get-FileHash "C:\\CAMINHO\\PING-Mobile-0.1.0-beta.1.apk" -Algorithm SHA256
```

No mesmo computador, após baixar o arquivo do GitHub, compare o hash para confirmar que os bytes são idênticos.

## Atualizações e assinatura

Cada nova build deverá receber nova tag, changelog e APK. Preserve as credenciais de assinatura Android gerenciadas pelo EAS para que futuras atualizações sejam instaláveis sobre as anteriores. Nunca adicione keystores, tokens EAS ou segredos de produção ao repositório.

## Site oficial

O site [pingsocial.online/download](https://www.pingsocial.online/download) pode apontar diretamente para o Asset da release por meio da variável de servidor `PING_ANDROID_BETA_APK_URL`. **Configure-a somente depois de publicar e verificar o arquivo**, usando uma URL HTTPS como:

```text
https://github.com/jhonatan-oliveiradev/ping-mobile-releases/releases/download/android-v0.1.0-beta.1/PING-Mobile-0.1.0-beta.1.apk
```

Este link só é válido depois que a tag e o asset com esses nomes existirem.

---

**Código-fonte:** repositório privado do PING. **Distribuição:** este repositório contém apenas instaladores e notas públicas.
