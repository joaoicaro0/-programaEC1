# SISTEMA DE VENDAS DE CELULARES 

## Nome dos Alunos 

João Guilherme De Araújo Dias MATRICULA : 20250067186

João Icaro Santos Bezerra  MATRICULA: 20250052601

Isabelle Silva Lisboa Da Conceição  MATRICULA: 20250052700


## Lógica do sistema

1. Iniciar o programa  
2. Solicitar nome do cliente  
3. Solicitar modelo do celular  
4. Solicitar preço do produto  
5. Solicitar forma de pagamento  
6. Verificar forma de pagamento  
7. Aplicar desconto ou taxa  
8. Calcular valor final  
9. Exibir resumo da compra  
10. Encerrar programa  

---

## Como executar

1. Instale o Python  
2. Execute o arquivo app.py com o comando:

python app.py

---

## Exemplo de uso

Entrada:
- Nome: João  
- Produto: iPhone 12  
- Preço: 1000  
- Pagamento: PIX  

Saída:
- Valor final com desconto aplicado  
- Exibição do resumo da compra


## Código do programa

```python
print("=== Sistema de Vendas ===")

# Entrada de dados
nome = input("Digite o nome do cliente: ")
modelo = input("Digite o modelo do celular: ")
preco = float(input("Digite o preço do celular: "))

print("\nForma de pagamento:")
print("1 - PIX (10% de desconto)")
print("2 - Cartão (5% de taxa)")
print("3 - Dinheiro (5% de desconto)")

opcao = int(input("Escolha a forma de pagamento: "))

# Processamento (switch em Python)
match opcao:
    case 1:
        desconto = preco * 0.10
        valor_final = preco - desconto
        metodo = "PIX"
    case 2:
        taxa = preco * 0.05
        valor_final = preco + taxa
        metodo = "Cartão"
    case 3:
        desconto = preco * 0.05
        valor_final = preco - desconto
        metodo = "Dinheiro"
    case _:
        print("Opção inválida!")
        valor_final = preco
        metodo = "Desconhecido"

# Saída de dados
print("\n=== Resumo da Compra ===")
print(f"Cliente: {nome}")
print(f"Produto: {modelo}")
print(f"Forma de pagamento: {metodo}")
print(f"Valor final: R$ {valor_final:.2f}")
```



## Conclusão

O desenvolvimento deste programa permitiu aplicar conceitos fundamentais da programação, como variáveis, entrada e saída de dados e estruturas condicionais.

Além disso, foi possível compreender como a lógica de programação pode ser utilizada para resolver problemas simples do cotidiano, como o cálculo de vendas e aplicação de descontos.
