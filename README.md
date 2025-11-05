# 🇧🇷 Validador de CPF em Python

Este script Python implementa a lógica oficial para calcular e verificar os dois dígitos verificadores (os dois últimos números) de um Cadastro de Pessoas Físicas (CPF) brasileiro.

Ele pode ser usado para verificar a validade estrutural de qualquer número de CPF, garantindo que os dígitos verificadores correspondem aos 9 dígitos iniciais.

## 🎯 Funcionalidade

O programa executa as seguintes etapas:

1.  **Isolamento:** Separa os 9 primeiros dígitos do CPF fornecido.
2.  **Cálculo do 1º Dígito:** Calcula o primeiro dígito verificador utilizando a multiplicação ponderada por uma contagem regressiva de 10 a 2.
3.  **Cálculo do 2º Dígito:** Utiliza os 9 dígitos iniciais mais o primeiro dígito calculado para determinar o segundo dígito verificador, usando uma contagem regressiva de 11 a 2.
4.  **Comparação:** Compara os dois dígitos verificadores calculados com os dígitos verificadores presentes no CPF original fornecido pelo usuário.
5.  **Resultado:** Informa se o CPF é estruturalmente **Válido** ou **Inválido**.

## 💻 Como Usar

### Pré-requisitos

Você precisa ter o **Python 3** instalado em sua máquina.

### Execução

1.  Salve o código em um arquivo chamado, por exemplo, `validador_cpf.py`.
2.  Abra o terminal ou prompt de comando.
3.  Navegue até o diretório onde você salvou o arquivo.
4.  Execute o script:

    ```bash
    python validador_cpf.py
    ```

### Alterando o CPF a Ser Verificado

Para testar diferentes CPFs, modifique a variável `cpf_enviado_usuario` no início do script:

```python
# O CPF deve ser fornecido como uma string de 11 dígitos.
cpf_enviado_usuario = '93846489069' # <--- Altere este valor para testar outros CPFs
