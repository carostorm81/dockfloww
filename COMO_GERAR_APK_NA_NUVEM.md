# Como gerar o APK sem Android Studio

Este projeto já vem com GitHub Actions configurado para gerar o APK na nuvem.
Você não precisa instalar Android Studio no computador.

## Passo 1: Criar um repositório no GitHub

1. Entre em https://github.com
2. Clique em **New repository**
3. Nome sugerido: `dockflow-supervisor-android`
4. Pode deixar privado
5. Clique em **Create repository**

## Passo 2: Enviar os arquivos

1. Dentro do repositório, clique em **uploading an existing file** ou **Add file > Upload files**
2. Envie todos os arquivos e pastas deste projeto
3. Confirme em **Commit changes**

Atenção: envie a pasta `.github` também. Ela é quem contém o robô que gera o APK.

## Passo 3: Gerar o APK

1. No repositório, abra a aba **Actions**
2. Clique em **Gerar APK DockFlow Supervisor**
3. Clique em **Run workflow**
4. Confirme novamente em **Run workflow**
5. Aguarde terminar. Geralmente demora alguns minutos.

## Passo 4: Baixar o APK

1. Quando a execução terminar com sinal verde, clique nela
2. Role até **Artifacts**
3. Baixe **DockFlow-Supervisor-APK**
4. Extraia o ZIP baixado
5. O arquivo será algo como `app-debug.apk`

## Passo 5: Instalar no celular

1. Envie o APK para o celular
2. Toque nele
3. Autorize instalar app desconhecido, se o Android pedir
4. Abra o app **DockFlow Supervisor**

## Importante

Este APK não tem chaves do Supabase. Ele abre apenas:

https://dockfloww.netlify.app/

As chaves e regras do DockFlow continuam protegidas na Netlify e no Supabase.
