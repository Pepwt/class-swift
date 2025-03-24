# class-swift


// main.swift

// Importando o arquivo Enfermeira.swift
import Foundation

// Instanciando um objeto da classe Enfermeira
let enfermeira = Enfermeira(nome: "Maria Silva", salario: 4500.75, trabalhaNoite: true, idade: 30)

// Exibindo as informações da enfermeira
enfermeira.exibirInformacoes()

---------------------------------------------------------------------------------------------------------------------------


// Enfermeira.swift

// Definindo a classe Enfermeira
class Enfermeira {
    // Atributos da classe
    var nome: String
    var salario: Float
    var trabalhaNoite: Bool
    var idade: Int
    
    // Inicializador (Construtor)
    init(nome: String, salario: Float, trabalhaNoite: Bool, idade: Int) {
        self.nome = nome
        self.salario = salario
        self.trabalhaNoite = trabalhaNoite
        self.idade = idade
    }
    
    // Método para exibir informações da enfermeira
    func exibirInformacoes() {
        print("Nome: \(nome)")
        print("Salário: R$ \(salario)")
        print("Trabalha à Noite: \(trabalhaNoite ? "Sim" : "Não")")
        print("Idade: \(idade)")
    }
}
