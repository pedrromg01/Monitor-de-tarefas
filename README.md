# Monitoramento de Sistema

![Demonstração do Projeto](https://github.com/pedrromg01/Monitor-de-tarefas/blob/main/monitor.js%20-%20Monitor%20SO%20-%20Visual%20Studio%20Code%202025-03-25%2023-38-22%20(1).gif)


## Descrição

Este projeto é um monitor de sistema desenvolvido em Node.js que coleta informações sobre o sistema operacional, arquitetura, modelo do processador, tempo de atividade e uso de memória RAM. Os dados são exibidos no console e salvos em um arquivo de log.

## Bibliotecas Utilizadas

O projeto utiliza módulos nativos do Node.js para acessar informações do sistema e manipular arquivos:

- **os**: Coleta informações sobre o sistema operacional, como plataforma, arquitetura, modelo do processador, tempo de atividade e uso de memória.
- **fs**: Permite interagir com o sistema de arquivos, sendo utilizado para criar diretórios e armazenar logs.
- **path**: Facilita a manipulação de caminhos de arquivos e diretórios.

## Funcionalidades

- Coleta dados do sistema operacional.
- Exibe as informações no console de forma clara.
- Salva os logs em um arquivo para análise futura.
- Atualiza as informações a cada segundo.

## Instalação e Execução

1. Certifique-se de ter o [Node.js](https://nodejs.org/) instalado.
2. Clone este repositório:
   ```sh
   git clone https://github.com/seu-usuario/seu-repositorio.git
   ```
3. Navegue até o diretório do projeto:
   ```sh
   cd nome-do-projeto
   ```
4. Execute o script:
   ```sh
   node index.js
   ```

## Estrutura do Código

### `getSystemInfo()`
Esta função coleta informações do sistema, como:
- Sistema operacional
- Arquitetura do processador
- Modelo do processador
- Tempo de atividade formatado em dias, horas, minutos e segundos
- Memória total e uso de RAM em GB e porcentagem

### `printLog(info)`
Esta função imprime no console os detalhes do sistema de forma organizada e clara.

### `saveLog(info)`
Esta função salva os logs coletados em um arquivo `log.txt` dentro do diretório `/log`. Caso o diretório não exista, ele será criado automaticamente.

### `setInterval()`
O código é executado a cada segundo para manter as informações sempre atualizadas.

## Melhorias Futuras

- Implementar suporte a exportação de logs em formatos diferentes (JSON, CSV, etc.).
- Criar uma interface web para visualização dos dados em tempo real.
- Adicionar suporte a notificações caso o uso da memória RAM ultrapasse um limite configurável.

## Contribuição

Sinta-se à vontade para contribuir com melhorias e novas funcionalidades. Para isso:
1. Faça um fork do repositório.
2. Crie uma nova branch:
   ```sh
   git checkout -b minha-melhoria
   ```
3. Faça as alterações e commit:
   ```sh
   git commit -m "Adiciona nova funcionalidade X"
   ```
4. Envie as mudanças:
   ```sh
   git push origin minha-melhoria
   ```
5. Abra um Pull Request para revisão.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---
