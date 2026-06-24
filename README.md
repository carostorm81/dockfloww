# DockFlow Supervisor Android

Projeto Android para gerar o APK do supervisor do DockFlow.

URL configurada no app:

```text
https://dockfloww.netlify.app/
```

## O que este app faz

- Abre o DockFlow em modo app Android.
- Mantém login pelo próprio DockFlow.
- Usa o perfil supervisor que já existe no sistema.
- Permite receber, atrasar, aguardar descarga e registrar divergência.
- Usa permissões de internet, vibração e notificação.
- Não coloca nenhuma chave Supabase dentro do APK.
- O app conversa apenas com a URL publicada na Netlify.

## Como gerar o APK no Android Studio

1. Abra o Android Studio.
2. Clique em **Open**.
3. Selecione a pasta deste projeto: `dockflow_supervisor_android`.
4. Aguarde o Gradle sincronizar.
5. Vá em **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. Quando terminar, clique em **locate** para encontrar o APK.

O APK geralmente fica em:

```text
app/build/outputs/apk/debug/app-debug.apk
```

## Para instalar no celular

1. Envie o APK para o Android.
2. Toque no arquivo.
3. Autorize instalação de app desconhecido, se o Android pedir.
4. Abra o app **DockFlow Supervisor**.

## Observações importantes

- O app depende do DockFlow publicado funcionar corretamente em `https://dockfloww.netlify.app/`.
- As variáveis Supabase continuam somente na Netlify.
- Notificação com app fechado exige Web Push nativo/FCM. Este app já prepara permissões e vibração para o uso com o DockFlow aberto.

## Desenvolvido por OWLLTECH.

## Gerar APK pela nuvem, sem Android Studio

Este pacote também inclui GitHub Actions em:

```text
.github/workflows/build-apk.yml
```

Com isso, você pode subir o projeto no GitHub e gerar o APK online, sem instalar Android Studio. Veja o arquivo:

```text
COMO_GERAR_APK_NA_NUVEM.md
```
