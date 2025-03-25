// Classe base Veiculo
class Veiculo {
    private String marca;
    private String modelo;
    private int ano;

    // Construtor
    public Veiculo(String marca, String modelo, int ano) {
        this.marca = marca;
        this.modelo = modelo;
        this.ano = ano;
    }

    // Método para exibir informações do veículo
    public void exibirInfo() {
        System.out.println("Marca: " + marca);
        System.out.println("Modelo: " + modelo);
        System.out.println("Ano: " + ano);
    }

    // Método para simular o som do veículo
    public void fazerSom() {
        System.out.println("Som genérico de veículo");
    }
}

// Classe Carro que herda de Veiculo
class Carro extends Veiculo {
    private int numeroPortas;

    // Construtor
    public Carro(String marca, String modelo, int ano, int numeroPortas) {
        super(marca, modelo, ano);
        this.numeroPortas = numeroPortas;
    }

    // Sobrescrevendo o método exibirInfo para incluir informações específicas do carro
    @Override
    public void exibirInfo() {
        super.exibirInfo();
        System.out.println("Número de portas: " + numeroPortas);
    }

    // Sobrescrevendo o método fazerSom para o carro
    @Override
    public void fazerSom() {
        System.out.println("Vrum Vrum (Som de carro)");
    }
}

// Classe Moto que herda de Veiculo
class Moto extends Veiculo {
    private boolean possuiPartidaEletrica;

    // Construtor
    public Moto(String marca, String modelo, int ano, boolean possuiPartidaEletrica) {
        super(marca, modelo, ano);
        this.possuiPartidaEletrica = possuiPartidaEletrica;
    }

    // Sobrescrevendo o método exibirInfo para incluir informações específicas da moto
    @Override
    public void exibirInfo() {
        super.exibirInfo();
        System.out.println("Possui partida elétrica: " + (possuiPartidaEletrica ? "Sim" : "Não"));
    }

    // Sobrescrevendo o método fazerSom para a moto
    @Override
    public void fazerSom() {
        System.out.println("Bibi Bibi (Som de moto)");
    }
}

// Classe principal para testar o sistema
public class Main {
    public static void main(String[] args) {
        // Criando objetos de Carro e Moto
        Veiculo carro = new Carro("Toyota", "Corolla", 2020, 4);
        Veiculo moto = new Moto("Honda", "CBR 600", 2019, true);

        // Usando polimorfismo para chamar métodos específicos de cada classe
        System.out.println("Informações do Carro:");
        carro.exibirInfo();
        carro.fazerSom();

        System.out.println("\nInformações da Moto:");
        moto.exibirInfo();
        moto.fazerSom();
    }
}
