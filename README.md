# Calculadora-em-python
Uma calculadora que fiz programando em python ainda falta muita coisa pois sou iniciante comecei no python fa poucos dias 

nome = input("porfavor digite seu nome:\n")

print(f"\n seja bem-vindo,{nome}\n")
resposta = int(input(f"{nome} voce deseja realizar alguma operacao matematica? \nse sim \ndigite 1 \nse nao digite 2\n"))
if resposta == 1:
    while True:
        print(f"\n{nome} digite dois mumeros logo apos escolha o metodo de solucao.\n")

        num1 = int(input("digite um valor:"))

        num2 = int(input(f"\n{nome} digite so mais um numero"))

        print(f"\nok {nome} agora escolha um metodo de solucao\n 1 para somar\n 2 para subtrair\n 3 para dividir  \n4 para multiplicar\n 0 para sair")

        msg_2 = int(input(f"\nescolha uma das opcoes!"))

        if msg_2 == 1:
            res_1 = num1 + num2
            print(f"\n{nome} o resultado da soma dos numero obitidos e {res_1}")
            res_10 = bool(input(f"voce deseja continuar?"))
            if res_10 == False:
                print("obrigado por usar")
                break
        elif msg_2 == 2:
            res_2 = num1 - num2
            print(f"\n{nome} o resultado da subtracao dos numeros selecionados e {res_2}")
            res_9 = bool(input(f"deseja continuar"))
            if res_9 == False:
                print("obrigado por usar")
                break

        elif msg_2 == 3:
            if num2 == 0:
                print(f"\n{nome} a divisao por zero nao e valida")
            else:
                res_3 = num1 / num2

                print(f"\n{nome} a divisao dos numeros escolhidos equivalem a {res_3}")
                res_8 = bool(input("\ndeseja continuar?"))
                if res_8 == False:
                    print("\nobrigado por usar")
                    break

        elif msg_2 == 4:
            res_4 = num1 * num2

            print(f"\na multiplicacao de {num1} para {num2} equivale a {res_4}")
            res_7 = int(input("\ndeseja continuar?digite 1 para sim e 2 para nao"))
            if res_7 == 2:
                print("\nobrigado por usar")
                break
            if res_7 != 1 or 2:
                print(f"\n digite apenas os mumeros listados! reinicie o progama")
                break
        else:
            print(f"\nvolte sempre {nome}")
            break
if resposta == 2:
    print(f"\n{nome} volte sempre") 
if resposta != 1 or 2:
    print(f"\n digite apenas os numeros listados,\nreinicie o progama e tente novamente")
    
