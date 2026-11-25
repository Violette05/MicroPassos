# MicroPassos Android

Primeira versão funcional do MicroPassos, feita com Kotlin e Jetpack Compose.

## O que já funciona
- Tela inicial com nível, XP e progresso.
- Criação de jornadas.
- Geração local de três passos iniciais por jornada.
- Conclusão de missões com recompensa de 10 XP.
- Tela de jornadas e tela de conquistas.
- Salvamento local de jornadas e XP usando SharedPreferences.
- Workflow do GitHub Actions para compilar o APK na nuvem.

## Requisitos para compilação local
- JDK 17
- Android SDK 35
- Gradle 8.9

## Gerar APK pela nuvem usando apenas o celular
1. Extraia este ZIP no celular.
2. Crie uma conta no GitHub, se ainda não tiver.
3. Crie um repositório novo chamado `MicroPassos`.
4. Envie os arquivos e pastas deste projeto para a raiz do repositório (incluindo a pasta oculta `.github`).
5. No GitHub, abra a aba **Actions**.
6. Se necessário, confirme a ativação dos workflows.
7. Selecione **Build MicroPassos APK** e toque em **Run workflow**.
8. Quando terminar, abra a execução e baixe o artefato `MicroPassos-debug-apk`.
9. Extraia o ZIP do artefato e instale `app-debug.apk` no Android. Talvez seja necessário permitir instalação pelo navegador ou gerenciador de arquivos.

## Observações
- Este é um APK de depuração, adequado para testes. Para publicar na Play Store será necessário configurar assinatura de lançamento e revisar os requisitos de publicação.
- O projeto ainda não usa IA online. A criação inicial das missões usa modelos locais simples, sem custo de API.
- A sequência diária está apresentada como indicador inicial; o cálculo automático de dias consecutivos será implementado em uma próxima versão.
