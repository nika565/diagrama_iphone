# Diagrama do Componente iPhone
### Tarefa do Bootcamp de Java da DIO
Este é o diagrama UML do componente iPhone, incluindo suas funcionalidades:

```mermaid
classDiagram
    class IReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }

    class IAparelhoTelefonico {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class INavegadorInternet {
        +exibirPagina(String url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    class iPhone {
        +reprodutorMusical: IReprodutorMusical
        +aparelhoTelefonico: IAparelhoTelefonico
        +navegadorInternet: INavegadorInternet
    }

    iPhone ..|> IReprodutorMusical
    iPhone ..|> IAparelhoTelefonico
    iPhone ..|> INavegadorInternet
