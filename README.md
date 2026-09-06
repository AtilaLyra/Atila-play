# ATILA PLAY V2.1

Cliente Android/Android TV para catálogos e reprodução de fontes fornecidas pelo usuário.

## Inclui
- Kotlin + Jetpack Compose
- Room para fontes, catálogo, favoritos, histórico e EPG
- parser M3U/M3U8
- sincronizador de fontes
- Media3/ExoPlayer
- controle parental com PIN inicial `0000`
- Home preparada para animes, canais, filmes e séries
- estrutura para Android TV/TV Box

## Observação
O projeto não incorpora listas, credenciais ou conteúdo protegido de terceiros e não implementa bypass de DRM/autenticação. Use apenas fontes que você esteja autorizado a utilizar.

## Compilação
Abra a pasta no Android Studio com Android SDK 35 e JDK 17. Gere o APK pelo menu Build.

## Build pelo celular

O projeto inclui `.github/workflows/build-apk.yml`. Depois de colocar o projeto em um repositório GitHub, abra **Actions**, selecione **Build ATILA PLAY APK** e execute **Run workflow**. O workflow usa JDK 17 e Gradle 8.10, gera o APK debug e também um APK release sem assinatura, e publica ambos como artefatos do workflow.

Para uma versão release assinada, configure posteriormente um keystore privado como GitHub Actions Secret e associe-o ao `signingConfig` do Gradle. Nunca coloque a chave de assinatura ou senhas dentro do repositório.
