# Aperta&Solta

Aplicativo em produção 

# Integração Flutter Module

O objetivo dessa tasks é viabilizar o uso de módulos Flutter em projetos nativos em produção aumentando assim a produtividade do time.

### Cenários

Atualmente contamos com dois repositórios um nativo android outro nativo ios com a criação do projeto em flutter teremos um terceiro repositório e este será independente dos outros repositórios.

**Como funcionará tudo isso?**

Basicamente será construído em Flutter a tela a ser susbistuido ou a nova feature. O app que será submetido na loja ainda será o app nativo porém dentro deles terá fragmentos contendo o módulo em Flutter. 

Todas features que forem construídas em Flutter e possuir uma dependência da parte nativa(vir diretamente dela) para que funcione devermos construir um bridge de comunicação entro a parte nativa e o Flutter existe várias formas de implementar, isso porém temos que saber que ainda não é possível fazer stream de um objeto completo a transmissão de dados ocorre a partir de dados primitivos. 

- Tabela de dados para transmissão (swift e kotlin)
    
    ![codec_swift.png](Aperta&Solta%20ecf31f17cb1e4b5e9573efb2bf23f64f/codec_swift.png)
    
    ![codec_kotlin.png](Aperta&Solta%20ecf31f17cb1e4b5e9573efb2bf23f64f/codec_kotlin.png)
    
    - 

Então um dos dados mais importante que o Flutter precisa ter acesso é o token para que possa ser usado no header da requisições que será realizadas em Flutter. 

Setup IOS

rvm

rvm install 2.7.1 --with-out-ext=fiddle