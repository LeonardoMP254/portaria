# 🏢 Sistema de Portaria Inteligente - TechZone
## 📌 Descrição

Este projeto foi desenvolvido como um protótipo de um **Sistema de Portaria Inteligente** para a empresa fictícia **TechZone**.
O objetivo é validar se um colaborador pode entrar no prédio com base no **nome informado** e no **horário de chegada**.

O sistema simula regras reais de acesso utilizadas em empresas de tecnologia, aplicando conceitos básicos de **JavaScript**, como:

- Arrays

- Condições (if...else)

- Operadores lógicos (&&)

- Manipulação de dados do usuário

---

## 🧠 Regras de Negócio

O sistema segue as seguintes validações:

### 1 📋 Banco de Dados

- Existe uma lista (Array) com os nomes autorizados:

```js

["Ana", "Carlos", "Marta", "João"]
```

### 2 🔍 Verificação de Identidade

- SE o nome digitado estiver na lista → acesso permitido

- SENÃO → acesso negado com a mensagem:

```

Acesso Negado: Usuário não cadastrado
```

### 3 ⏰ Regra de Horário (Diferencial)

- Mesmo autorizado, o colaborador só pode entrar antes das 22h

- Regra lógica aplicada:
```

estaNaLista == true && horario < 22
```
---
## 💻 Exemplo de Código
```
const autorizados = ["Ana", "Carlos", "Marta", "João"];

let nome = prompt("Digite seu nome:");
let horario = new Date().getHours();

if (autorizados.includes(nome)) {
    if (horario < 22) {
        alert("Acesso Permitido: Bem-vindo(a) " + nome);
    } else {
        alert("Acesso Negado: Fora do horário permitido");
    }
} else {
    alert("Acesso Negado: Usuário não cadastrado");
}
```
---
## 🚀 Como Executar

**1.** Abra o arquivo index.html

**2.** Execute o script no navegador

**3.** Digite o nome do colaborador

**4.** O sistema validará:

- Se o nome está autorizado

- Se está dentro do horário permitido
---
## 🎯 Objetivo da Atividade

Praticar conceitos fundamentais de JavaScript:

- Estruturas condicionais

- Arrays

- Validação de dados

- Operadores lógicos

- Simulação de regras de negócio reais

--- 
## 📚 Aprendizados

Com este projeto foi possível aprender:

- Como verificar se um valor existe em um Array (includes)

- Como usar if...else aninhado

- Como trabalhar com horário usando Date()

- Como criar validações semelhantes a sistemas reais de empresas

##👨‍💻 Autor

Desenvolvido por: **Leonardo** 
Atividade acadêmica de JavaScript 💙
