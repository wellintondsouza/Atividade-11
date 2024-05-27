#include <iostream>
#include <string>

using namespace std;

// Função para cadastrar as notas de um aluno
void cadastrarNotas(string& nome, float notas[]) {
    cout << "Escreva o nome do aluno:\n ";
    cin >> nome;
    
    cout << "Escreva as notas do aluno:\n ";
    for (int i = 0; i < 4; ++i) {
        cin >> notas[i];
    }
}

// Função para calcular a média de um aluno e determinar seu status
void calcularMediaEStatus(const string& nome, const float notas[]) {
    float soma = 0;
    for (int i = 0; i < 4; ++i) {
        soma += notas[i];
    }
    float media = soma / 4;
    
    cout << "A media do aluno " << nome << " e " << media << endl;
    
    if (media < 4) {
        cout << "O aluno esta reprovado\n" << endl;
    } else if (media >= 6) {
        cout << "O aluno esta aprovado\n" << endl;
    } else {
        cout << "O aluno esta de recuperacao\n" << endl;
    }
}

int main() {
    const int NUM_ALUNOS = 5;
    string nomes[NUM_ALUNOS];
    float notas[NUM_ALUNOS][4];

    int opcao;
    do {
        cout << "MENU" << endl;
        cout << "1- Cadastro das Notas dos Alunos" << endl;
        cout << "2- Alteracao das Notas" << endl;
        cout << "3- SAIR" << endl;
        cout << "Escolha uma opcao: ";
        cin >> opcao;

        switch (opcao) {
            case 1:
                cout << "CADASTRO DE NOTAS DOS ALUNOS" << endl;
                for (int i = 0; i < NUM_ALUNOS; ++i) {
                    cadastrarNotas(nomes[i], notas[i]);
                    calcularMediaEStatus(nomes[i], notas[i]);
                }
                break;
            case 2:
                cout << "ALTERACAO DE NOTAS\n" << endl;
                for (int i = 0; i < NUM_ALUNOS; ++i) {
                    cadastrarNotas(nomes[i], notas[i]);
                    calcularMediaEStatus(nomes[i], notas[i]);
                }
                break;
            case 3:
                cout << "Saindo..." << endl;
                break;
            default:
                cout << "Opcao invalida! Tente novamente.\n" << endl;
        }
    } while (opcao != 3);

    return 0;
}
