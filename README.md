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
   <li><strong>Solução 3 (boa)</strong>: tratamento de exceções</li>
</ul>

