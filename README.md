# Pedra-papel-tesoura.py
# Código em Python do jogo "joquempô"
import random
p1 = input('Pedra, papel ou tesoura?').lower()
print(p1)
p2 = random.choice(['pedra', 'papel', 'tesoura']).lower()
print(p2)
if p1=='pedra' and p2=='tesoura':
    print('Pedra quebra tesoura. P1 ganhou.')
elif p1=='tesoura' and p2=='papel':
    print('Tesoura corta o papel. P1 ganhou.')
elif p1=='papel' and p2=='pedra':
    print('Papel embrulha pedra. P1 ganhou.')
elif p1=='tesoura' and p2=='pedra':
    print('Pedra quebra tesoura. P2 ganhou.')
elif p1=='papel' and p2=='tesoura':
    print('Tesoura corta o papel. P2 ganhou.')
elif p1=='pedra' and p2=='papel':
    print('Papel embrulha pedra. P2 ganhou.')
elif p1=='papel' and p2=='papel':
    print('Papel com papel. Empate.')
elif p1=='pedra' and p2=='pedra':
    print('Pedra com pedra. Empate.')
elif p1=='tesoura' and p2=='tesoura':
    print('Tesoura com tesoura. Empate.')
