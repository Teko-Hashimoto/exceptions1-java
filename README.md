# Curso: Java COMPLETO - Programação Orientada a Objetos
## Professor <a href="https://github.com/acenelio">Nelio Alves</a> 
## Aula: Tratamento de exceções

## Resumo da aula

<ul>
  <li><strong>Solução 1 (muito ruim)</strong>: lógica de validação no programa principal
    <ul>
      <li>Lógica de validação não delegada à reserva</li>
    </ul>
  </li>
  <hr>
  <li><strong>Solução 2 (ruim)</strong>: método retornando string</li>
  <ul>
      <li>A semântica da operação é prejudicada
        <ul>
          <li>Retornar string não tem nada a ver com atualização de reserva</li>
          <li>E se a operação tivesse que retornar um string?</li>
        </ul>
      </li>
      <li>Ainda não é possível tratar exceções em construtores</li>
      <li>Ainda não há auxílio do compilador: o programador deve "lembrar" de verificar se houve 
erro</li>
      <li>A lógica fica estruturada em condicionais aninhadas</li>
    </ul>
  <hr>
   <li><strong>Solução 3 (boa)</strong>: tratamento de exceções</li>
    <ul>
      <li>Cláusula throws: propaga a exceção ao invés de trata-la</li>
      <li>Cláusula throw: lança a exceção / "corta" o método</li>
      <li>Exception: compilador obriga a tratar ou propagar</li>
      <li>RuntimeException: compilador não obriga</li>
      <li>O modelo de tratamento de exceções permite que erros sejam tratados de forma consistente e flexível, 
        <strong>usando boas práticas</strong></li>
      <li>Vantagens:
        <ul>
          <li>Lógica delegada</li>
          <li>Construtores podem ter tratamento de exceções</li>
          <li>Possibilidade de auxílio do compilador (Exception)</li>
          <li>Código mais simples. Não há aninhamento de condicionais: a qualquer momento que uma exceção for disparada, 
            a execução é interrompida e cai no bloco catch correspondente</li>
          <li>É possível capturar inclusive outras exceções de sistema</li>
        </ul>
      </li>
    </ul>
</ul>

