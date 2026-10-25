# Trabalho: GitHub e Pipeline de Feedback

**Componente curricular:** Desenvolvimento de Sistemas  
**Conteúdo:** Semana 21 — Aula 2: Pipeline de Feedback  
**Tema:** Cultura DevOps e Feedback Contínuo  

**Integrantes:**  
- Victor Hugo  
- Matheus Rocha  
- Ezequiel  

---

## 1. Introdução

O GitHub é uma plataforma de hospedagem de código que utiliza o Git (sistema de controle de versão). Ele permite armazenar projetos, registrar todas as alterações feitas no código e facilitar o trabalho em equipe.

Além de guardar o código, o GitHub se conecta diretamente com práticas de DevOps, principalmente através do **GitHub Actions**, que automatiza tarefas. Neste trabalho vamos mostrar como o GitHub se relaciona com o **Pipeline de Feedback** estudado na Aula 2.

## 2. O que é um Pipeline de Feedback?

É uma sequência automática de passos que valida o código toda vez que alguém faz uma alteração.

Fluxo básico (como visto na aula):

**Código → Build → Teste → Resultado**

O objetivo principal é descobrir o erro o mais rápido possível (mentalidade **fail fast**). Quanto mais cedo o erro aparece, mais barato e fácil de corrigir.

## 3. Etapas do Pipeline de Feedback

1. **Build**  
   Compila e prepara o código, verificando se ele “monta” corretamente.

2. **Test**  
   Executa testes automatizados (unitários e de integração) para validar se a lógica está funcionando.

3. **Monitor**  
   Acompanha o resultado e envia alertas automáticos para a equipe quando algo falha.

Ferramentas que fazem isso: **GitHub Actions** e **Jenkins**.

## 4. Como o GitHub se relaciona com o Pipeline de Feedback?

O GitHub não é só um “depósito de código”. Com o **GitHub Actions** é possível criar um pipeline que roda automaticamente toda vez que alguém faz um *commit* (envia alteração).

Exemplo prático:
- O desenvolvedor manda o código.
- O GitHub Actions inicia o pipeline.
- Roda o build e os testes.
- Mostra se deu ✅ sucesso ou ❌ erro.

Isso é exatamente o feedback rápido que a aula fala. O erro aparece em minutos, não em dias.

## 5. Mentalidade Fail Fast e Lead Time

**Fail Fast** = descobrir a falha o mais cedo possível.

**Lead Time** = tempo total desde a ideia até o código estar em produção.

A regra de ouro da aula:
> Quanto mais tarde um erro é descoberto, mais caro e complexo fica para corrigir.

O pipeline automatizado no GitHub reduz esse tempo e o custo do atraso.

## 6. Exemplo de fluxo em equipe

Imagine os três integrantes trabalhando no mesmo repositório:

1. Um deles altera o código e envia (commit + push).
2. O pipeline inicia automaticamente.
3. Build e testes rodam.
4. Se der erro, o GitHub mostra o resultado na hora.
5. A pessoa corrige e manda de novo.
6. O ciclo se repete até dar sucesso.

Isso é feedback contínuo na prática.

## 7. Benefícios

- Erros descobertos em minutos, não em dias
- Menos retrabalho
- Código de melhor qualidade
- Entregas mais seguras
- Trabalho em equipe mais organizado

## 8. Conclusão

O GitHub + GitHub Actions transforma o repositório em um pipeline de feedback real. Em vez de descobrir o erro só quando o sistema cai em produção (como no exemplo da sexta-feira da aula), o time recebe o resultado imediatamente.

Isso é o coração da cultura DevOps e do feedback contínuo: falhar rápido, corrigir rápido e entregar com mais segurança.

## Referências

- Material da Aula 2 – Semana 21 (SISANO1C3B4S21A2) – Educação Profissional Paulista
- Documentação GitHub Actions: https://docs.github.com/pt/actions
- AWS – O que é um pipeline de CI/CD: https://aws.amazon.com/pt/what-is/ci-cd-pipeline/
