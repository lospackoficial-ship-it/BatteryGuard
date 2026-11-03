# Battery Guard

App Android com root para proteger a bateria limitando a carga.

## Funcionalidades

- Pede permissão de root ao abrir
- Define porcentagem máxima para parar a carga (ex: 80%)
- Define porcentagem mínima para reativar a carga automaticamente (ex: 75%)
- Serviço em segundo plano com notificação permanente
- Funciona em Snapdragon (testa vários caminhos sysfs)
- Reinicia automaticamente após boot (se estava ativo)

## Como compilar

1. Abra a pasta no Android Studio (Hedgehog ou mais recente)
2. Aguarde o Gradle sincronizar (ele vai baixar a libsu)
3. Conecte um celular com root (Magisk / KernelSU recomendado)
4. Clique em Run

## Requisitos

- Android 8.0+ (API 26)
- Root (Magisk, KernelSU ou similar)
- Processador Snapdragon (outros também podem funcionar)

## Uso

1. Abra o app e conceda a permissão de root
2. Ajuste o limite máximo e o limite mínimo
3. Ative o switch "Ativar proteção de bateria"
4. Pronto. O app cuida do resto

## Observação importante

O caminho do sysfs pode variar entre modelos. O app tenta detectar automaticamente.
Se não funcionar no seu aparelho, abra um issue informando o modelo.
