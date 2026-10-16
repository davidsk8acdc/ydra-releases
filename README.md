# YDRA — distribuição

Repositório de distribuição da ferramenta de configuração e do firmware
da placa YDRA.

**Aqui não tem código-fonte.** Só os binários, nas Releases, e o
`versoes.json`, que é o arquivo que a ferramenta instalada consulta para
saber se há novidade.

## Para quem usa a ferramenta

Baixa o instalador mais recente em
[Releases](../../releases/latest) e instala. Não pede senha de
administrador — ele se instala dentro do seu usuário.

Depois disso a ferramenta se atualiza sozinha: quando você abre, ela
confere se saiu versão nova e pergunta se quer instalar.

O firmware da placa também. Quando sai um novo, a ferramenta baixa em
segundo plano e deixa pronto — na hora de atualizar a placa o caminho já
vem preenchido.

## Sobre o firmware publicado aqui

O firmware é **assinado**. A placa usa Secure Boot e não aceita binário
que não tenha a assinatura correta, então um .bin aqui não serve para
mais nada além de atualizar uma YDRA legítima.

## Etiquetas das Releases

```
ferramenta-X.Y.Z    instalador da ferramenta (Windows)
firmware-X.Y.Z      firmware.bin assinado
```

As duas correm separadas: sai firmware novo sem ferramenta nova, e
vice-versa.
