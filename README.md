function calcularRanking(vitorias, derrotas) {
    const saldoRankeadas = vitorias - derrotas;

    if (vitorias < 10) {
        return "Ferro";
    } else if (vitorias >= 10 && vitorias <= 20) {
        return "Bronze";
    } else if (vitorias > 20 && vitorias <= 50) {
        return "Prata";
    } else if (vitorias > 50 && vitorias <= 80) {
        return "Ouro";
    } else if (vitorias > 80 && vitorias <= 90) {
        return "Diamante";
    } else if (vitorias > 90 && vitorias <= 100) {
        return "Lendário";
    } else {
        return "Imortal";
    }
}

const vitorias = 90;
const derrotas = 10;
const resultado = calcularRanking(vitorias, derrotas);
console.log(resultado); 
