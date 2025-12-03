# Desafio - 3º Trimestre

## Problema 1: Sistema de Gerenciamento de Biblioteca

Contexto: Você está desenvolvendo um sistema de gerenciamento para uma pequena biblioteca. O sistema deve permitir adicionar livros, remover livros, buscar por categoria, e gerar relatórios.

### Requisitos:
1. Função para validar entrada do usuário: Crie uma função que valide se o usuário inseriu dados válidos (usando while).
2. Função para adicionar livro: Recebe o array de livros, nome do livro e categoria. Adiciona o livro ao array.
3. Função para remover livro: Recebe o array e o nome do livro. Remove o livro se encontrado.
4. Função para listar livros cadastrados.
5. Menu interativo: Use while para manter o programa rodando até o usuário sair. Use if...else aninhado para cada opção do menu.

Dados Iniciais:

```javascript
let livros = ["1984", "Dom Casmurro", "O Cortiço", "Grande Sertão Veredas"];
let categorias = ["Ficção Científica", "Romance", "Realismo", "Modernismo"];
```

> **DESAFIO:** O sistema deve permitir o usuário adicionar e remover livros, listar por categoria, e sempre validar as entradas. Implemente tudo isso com funções, loops e decisões aninhadas.


## Problema 2: Gestor de Notas e Médias de Alunos

Contexto: Um professor precisa de um sistema para registrar as notas dos seus 5 alunos em 4 bimestres, calcular médias e identificar alunos com desempenho baixo.

### Requisitos:
1. Função para validar notas: Valide se a nota está entre 0 e 10 (use while).
2. Função para adicionar notas: Insira as 4 notas de cada aluno usando for.
3. Função para calcular média: Use for para somar as notas e calcular a média.
4. Função para classificar desempenho: Use if...else aninhado:
	 - Média >= 9: Excelente
	 - Média >= 7: Bom
	 - Média >= 5: Regular
	 - Média < 5: Insuficiente
5. Função para gerar relatório: Mostre o nome, notas, média e classificação de cada aluno.

Dados Iniciais:

```javascript
let alunos = ["João", "Maria", "Pedro", "Ana", "Carlos"];
let notas = [
	// cada elemento é um array com 4 notas, ex: [8, 7.5, 9, 10]
];
```

> **DESAFIO:** Implemente um sistema completo onde o professor possa cadastrar notas, remover um aluno se necessário, visualizar relatórios e tudo validado adequadamente.
## Problema 3: Sistema de Estoque de Produtos com Preço

Contexto: Uma loja pequena precisa gerenciar seu estoque. O sistema deve permitir adicionar produtos, remover, ajustar preços, e gerar relatórios de produtos caros, baratos e com baixo estoque.

### Requisitos:
1. Função para validar entrada: Valide quantidade e preço (use while para re-solicitar dados inválidos).
2. Função para adicionar produto: Adicione nome, quantidade e preço ao array.
3. Função para remover produto: Remova um produto específico do array.
4. Função para listar produtos por faixa de preço: Use for e if...else para filtrar:
	- Produtos baratos (< R$ 50)
	- Produtos médios (R$ 50 a R$ 150)
	- Produtos caros (> R$ 150)
5. Função para alertar sobre estoque baixo: Identifique produtos com quantidade <= 5.
6. Menu interativo: Use while com if...else aninhado para navegação.

Dados Iniciais:

```javascript
let nomeProdutos = ["Arroz", "Feijão", "Açúcar", "Sal"];
let quantidades = [50, 30, 20, 15];
let precos = [3.50, 8.00, 4.50, 2.00];
```

> **DESAFIO:** Crie um sistema robusto que valide todas as entradas, permita manipulação completa do estoque e gere relatórios detalhados.

## Problema 4: Simulador de Vendas com Comissão

Contexto: Uma empresa tem 3 vendedores. Você deve criar um sistema que registre as vendas de cada vendedor ao longo de 5 dias, calcule o total de vendas e a comissão baseada em faixas de desempenho.

### Requisitos:
1. Função para validar valor de venda: Valide se o valor é positivo (use while).
2. Função para registrar vendas: Use for para registrar vendas de 5 dias para cada vendedor. Armazene em um array.
3. Função para calcular total de vendas: Some todas as vendas de cada vendedor usando for.
4. Função para calcular comissão: Use if...else aninhado:
	- Vendas < R$ 5000: 5% de comissão
	- Vendas R$ 5000 a R$ 10000: 10% de comissão
	- Vendas R$ 10000 a R$ 15000: 15% de comissão
	- Vendas > R$ 15000: 20% de comissão

Dados Iniciais:

```javascript
let vendedores = ["Carlos", "Ana", "Pedro"];
let vendas = [[], [], []]; // Array para armazenar vendas de cada vendedor
```

> **DESAFIO:** Implemente um sistema onde o gerente possa inserir vendas, validar dados, calcular comissões e visualizar um ranking de desempenho.

## Problema 5: Gerenciador de Tarefas com Prioridade e Prazos

Contexto: Você está criando um aplicativo de gerenciamento de tarefas. O sistema deve permitir adicionar tarefas com prioridade e prazo, remover tarefas concluídas, e gerar relatórios de tarefas por urgência.

### Requisitos:
1. Função para validar prioridade: Aceite apenas "alta", "média" ou "baixa" (use while).
2. Função para adicionar tarefa: Adicione descrição, prioridade e dias restantes a um array.
3. Função para remover tarefa: Remova uma tarefa pelo índice ou descrição.
4. Menu com while e if...else aninhado para adicionar, remover, visualizar e sair.

Dados Iniciais:

```javascript
let tarefas = ["Fazer relatório", "Enviar email", "Estudar JavaScript"];
let prioridades = ["alta", "média", "baixa"];
let diasRestantes = [2, 5, 10];
```

> **DESAFIO:** Crie um sistema funcional completo de gerenciamento de tarefas com validação rigorosa e categorização inteligente.

## Problema 6: Sistema de Reservas de Restaurante

Contexto: Um restaurante precisa gerenciar suas reservas. O sistema deve permitir reservar mesas, cancelar reservas, visualizar mesas disponíveis e gerar relatórios de ocupação.

### Requisitos:
1. Função para validar entrada: Valide nome (não vazio), horário (6 a 22h), número de pessoas (1 a 20) usando while.
2. Função para fazer reserva: Adicione a reserva ao array se houver mesa disponível.
3. Função para cancelar reserva: Remova uma reserva pelo nome.
4. Função para listar mesas disponíveis: Use for e if...else para identificar:
	- Mesas vazias (totalmente disponíveis)
	- Mesas meio-ocupadas
	- Mesas cheias
5. Menu interativo com while e if...else aninhado.

Dados Iniciais:

```javascript
let reservas = ["João - 19:00", "Maria - 20:00"];
let horarios = [19, 20];
let pessoasReservadas = [4, 6];
let mesasDisponiveis = 10;
```

> **DESAFIO:** Implemente um sistema robusto de reservas com validação completa e relatórios de ocupação em tempo real.

## Problema 7: Calculadora de Desconto com Categorias de Clientes

Contexto: Uma loja precisa de um sistema que calcule o preço final de uma compra baseado na categoria do cliente e valor total. O sistema deve permitir adicionar itens, remover itens e calcular o total com desconto.

### Requisitos:
1. Função para validar entrada: Valide categoria de cliente (use while - apenas "Premium", "Gold" ou "Standard").
2. Função para validar preço: Valide se o preço é positivo.
3. Função para adicionar item ao carrinho: Use push() para adicionar nome e preço.
4. Função para remover item: Remova um item do carrinho pelo índice.
5. Função para calcular total: Use for para somar todos os itens.
6. Função para aplicar desconto: Use if...else aninhado:
	- Premium: 20% de desconto
	- Gold: 15% de desconto
	- Standard: 5% de desconto
	- (Mas se o total for > R$ 500, adicione 5% extra de desconto)
7. Função para gerar recibo: Mostre itens, total, desconto e preço final.

Dados Iniciais:

```javascript
let itensCarrinho = ["Camiseta", "Calça", "Meia"];
let precos = [50, 150, 15];
let categoriaCliente = ""; // Será preenchida pelo usuário
```

> **DESAFIO:** Crie um sistema de e-commerce que valide dados, manipule o carrinho corretamente e calcule descontos complexos.

## Problema 8: Analisador de Performance de Atletas

Contexto: Você está desenvolvendo um sistema para analisar o desempenho de 4 atletas em 6 competições. O sistema deve registrar pontos, calcular médias, identificar o melhor desempenho e remover atletas se necessário.

### Requisitos:
1. Função para validar pontuação: Valide se a pontuação está entre 0 e 100 (use while).
2. Função para registrar pontos: Use for para registrar pontos de cada atleta em 6 competições.
3. Função para calcular média: Use for para somar e dividir.
4. Função para encontrar melhor desempenho: Compare todas as médias usando for.
5. Função para remover atleta: Remova um atleta do ranking se ele pedir para sair.
6. Função para gerar relatório completo: Mostre todos os atletas, médias, rankings e desempenho.

Dados Iniciais:

```javascript
let atletas = ["João", "Maria", "Pedro", "Ana"];
let pontos = [[], [], [], []]; // 6 competições para cada atleta
```

> **DESAFIO:** Crie um sistema de análise estatística que valide dados, calcule múltiplas métricas e gere relatórios comparativos.

## Problema 9: Sistema de Controle de Frequência Escolar

Contexto: Uma escola precisa de um sistema para controlar a frequência de 6 alunos ao longo de 20 dias de aula. O sistema deve registrar presença/ausência, calcular percentual de frequência e identificar alunos com risco de reprovação por falta.

### Requisitos:
1. Função para validar entrada: Valide se o usuário digitou "P" (presente) ou "F" (faltou) (use while).
2. Função para registrar frequência: Use for para registrar 20 dias de frequência para cada aluno.
3. Função para calcular percentual de frequência: Use for para contar presenças e calcular percentual.
4. Função para listar alunos em risco: Identifique e mostre quem está com frequência < 60%.
5. Função para permitir adicionar/remover alunos: Manipule o array de alunos.
6. Função para gerar relatório: Mostre cada aluno, dias presentes, dias ausentes, percentual e classificação.

Dados Iniciais:

```javascript
let alunos = ["João", "Maria", "Pedro", "Ana", "Carlos", "Beatriz"];
let frequencia = [[], [], [], [], [], []]; // 20 dias para cada aluno
let totalDias = 20;
```

> **DESAFIO:** Implemente um sistema de controle de frequência robusto com validação rigorosa, cálculos precisos e relatórios detalhados que ajudem a identificar riscos.