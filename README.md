// --- Desafio Classificador de Nível de Herói ---

// 1. Variáveis
// Armazenamos o nome e a quantidade de XP do nosso herói.
// Sinta-se à vontade para alterar esses valores e testar diferentes níveis!
let nomeHeroi = "Aragorn";
let xpHeroi = 8500;

// Variável para armazenar o nível, que será definida pela estrutura de decisão
let nivelHeroi;

// 2. Estrutura de Decisão (if-else if-else)
// Usamos uma cadeia de 'if-else if' para verificar as faixas de XP.
// A verificação é feita em ordem, da menor para a maior, o que simplifica a lógica.

if (xpHeroi <= 1000) {
    nivelHeroi = "Ferro";
} else if (xpHeroi <= 2000) {
    // Se chegou aqui, o XP é > 1000
    nivelHeroi = "Bronze";
} else if (xpHeroi <= 5000) {
    // Se chegou aqui, o XP é > 2000
    nivelHeroi = "Prata";
} else if (xpHeroi <= 7000) {
    // Se chegou aqui, o XP é > 5000
    nivelHeroi = "Ouro";
} else if (xpHeroi <= 8000) {
    // Se chegou aqui, o XP é > 7000
    nivelHeroi = "Platina";
} else if (xpHeroi <= 9000) {
    // Se chegou aqui, o XP é > 8000
    nivelHeroi = "Ascendente";
} else if (xpHeroi <= 10000) {
    // Se chegou aqui, o XP é > 9000
    nivelHeroi = "Imortal";
} else {
    // Se nenhuma das condições anteriores for verdadeira, o XP é >= 10001
    nivelHeroi = "Radiante";
}

// 3. Saída
// Exibimos a mensagem final com o nome e o nível do herói.
// Usamos template literals (crases ``) para facilitar a inserção das variáveis no texto.
console.log(`O Herói de nome **${nomeHeroi}** está no nível de **${nivelHeroi}**`);
