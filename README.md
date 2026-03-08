function calcularRank(vitorias, derrotas) {
    let saldo = vitorias - derrotas
    let nivel

    if (vitorias <= 10) {
        nivel = "Ferro"
    } else if (vitorias <= 20) {
        nivel = "Bronze"
    } else if (vitorias <= 50) {
        nivel = "Prata"
    } else if (vitorias <= 80) {
        nivel = "Ouro"
    } else if (vitorias <= 90) {
        nivel = "Diamante"
    } else if (vitorias <= 100) {
        nivel = "Lendário"
    } else {
        nivel = "Imortal"
    }

    return `O Herói tem saldo de ${saldo} e está no nível ${nivel}`
}

let heroi = {
    nome: "Jogador",
    vitorias: 75,
    derrotas: 20
}

console.log(calcularRank(heroi.vitorias, heroi.derrotas))# projeto-logica-de-programa-o2
