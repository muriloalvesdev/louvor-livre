# Louvor Livre

Banco de letras de louvor **livre e gratuito** para uso em aplicações de igrejas, projetores, apps de culto e qualquer sistema que precise de letras de músicas gospel/worship em português.

## Como usar

### Catálogo completo
```
GET https://muriloalvesdev.github.io/louvor-livre/index.json
```

### Letra de uma música
```
GET https://muriloalvesdev.github.io/louvor-livre/louvores/{arquivo}.json
```

### Estrutura do index.json
```json
[
  {
    "file": "artista--nome-da-musica",
    "artist": "Nome do Artista",
    "title": "Nome da Música",
    "tone": "G"
  }
]
```

### Estrutura de cada louvor
```json
{
  "artist": "Nome do Artista",
  "title": "Nome da Música",
  "tone": "G",
  "lyrics": "Letra completa da música...",
  "tags": ["adoração", "avivamento"]
}
```

## Contribuindo

1. Fork este repositório
2. Crie um arquivo JSON em `louvores/` seguindo o padrão: `artista--nome-da-musica.json`
3. Adicione a entrada no `index.json`
4. Abra um Pull Request

### Padrão do nome do arquivo
- Tudo minúsculo
- Espaços viram `-`
- Artista e música separados por `--`
- Sem acentos
- Exemplo: `aline-barros--ressuscita-me.json`

## Licença

As letras pertencem aos seus respectivos autores e compositores. Este repositório é mantido para fins educacionais e de uso em cultos religiosos.

MIT License para o código/estrutura do projeto.
