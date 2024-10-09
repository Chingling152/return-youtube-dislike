Leia isso em outros idiomas: [русский](CONTRIBUTINGru.md), [Nederlands](CONTRIBUTINGnl.md), [Français](CONTRIBUTINGfr.md), [Türkçe](CONTRIBUTINGtr.md), [українська](CONTRIBUTINGuk.md), [Polski](CONTRIBUTINGpl.md)

# Bem-vindo ao Guia de contribuição do Return YouTube Dislikes

Obrigado por investir o seu tempo contribuindo para o nosso projeto! Todas as mudanças serão refletidas na proxima versão da extensão: (ou no [website](https://www.returnyoutubedislike.com/)).

## Vamos ao começo

Por favor use o Prettier com a configurações padrão de formatação.

#### Pré-requisitos

Você precisa ter node e npm instalado para criar a versão compilada do código.

Versões que usará quando estiver trabalhando nisso:

- node: 12.18.4
- npm: 6.14.6

Para criar o `bundled-content-script.js` que contem a maioria da lógica de negócio dessa extensão, você precisa instalar todas as dependências primeiro.

1. Vá para a raiz do repositório e execute:

```
npm install
```

2. Execute o seguinte comando para criar `bundled-content-script.js` que é usado no `manifest.json`

```
npm start // para criar um arquivo(s) de build e iniciar um observador de arquivos que faça hot-reloads ao salvar.

// ou

npm run build // para criar uma build para cria um arquivo de build 
```

Parabéns, você agora está pronto para desenvolver!

Se você é novato no desenvolvimento de extensões para o Chrome, ou precisa de ajuda, por favor veja [esse tutorial no YouTube](https://www.youtube.com/watch?v=mdOj6HYE3_0)

### Problemas

#### Abrindo um novo problema

Se voce tiver qualquer problema com a extensão, por favor pesquisa o que faz o problema antes de reporta-lo de fato. Se não houver, abra um probelma, usando o formulario de problema é recomendado mas não é uma obrigação.

#### Solucionando um problema

Se você tiver um problema que você acha que pode resolver, não seja tímido. Abra um PR com a correção e faça uma menção do problema que está corrigindo.

### Requisitação de Funcionalidade

#### Abrindo uma nova requisitação de funcionalidade

Se você tem alguma ideia para a extensão, sinta-se livre para abrir uma requisitação de funcionalidade, mas por favor pesquise isso antes para não perder seu tempo com sua sugestão. Usar o formulario de recurso é altamente recomendado mas não é um obrigação.

#### Implementando uma requisitação de funcionalidade

Se você achou uma funcionalidade que você acha que consegue implementar, não seja tímido. Abra um PR com a correção e tenha certeza de mencionar a feature que você está implementando.

### Que PRs nós aceitamos?

- Resolução de problemas.
- Implementação de funcionalidades.
- Erros de digitação ou palavras melhores e mais fáceis de usar.
- Contribuições para o Website.
