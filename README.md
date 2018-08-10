import math
def cosseno(n):
    if n==float or n==int:
        n = float(n)
        print('o valor do cosseno é: {:.3f}'.format(math.cos(n)))
        print('\n')
        return menu()
    else:
        print('Digite um valor válido')
        return menu()



def cotangente(x):
    print('O valor da cotangente é: {:.3f}'.format(float(math.cos(x)) / (math.sin(x))))
    print('\n')
    return menu()


def arcotangente(y):
    print('O valor do arco cotangente é: {:.3f}'.format(float(math.atan(1/y))))
    print('\n')
    return menu()




def menu():
    print('''Olá, pequeno gafanhoto, seja bem vindo a nossa calculadora!''')
    print('----------------MENU------------------')
    print('[1]Cosseno [2]Cotangente  [3] Arco Cotangente [0] Para sair da calculadora' )
    print('                                             ')
    calc = input('''Calculadora feita para calcular em radianos, Agora digite o numero correspondente ao que você deseja calcular:\n''')


    if calc == '1':
        return cosseno(input('Digite o valor para calcular o cosseno: '))


    elif calc == '2':
        return cotangente((float(input('Digite o valor para calcular a cotangente: '))))



    elif calc == '3':
        return arcotangente(float(input('Digite o valor para calcular o arco cotangente: ')))

    elif calc == '0':
        print('Obrigado, volte sempre!')




    else:
        print('Nenhuma função correspondente')
        print('\n')
        return menu()


menu()
