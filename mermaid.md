erDiagram
    EDITORA ||--o{ LIVRO : publica
    LIVRO ||--|{ LIVRO_AUTOR : contem
    AUTOR ||--|{ LIVRO_AUTOR : escreve

    EDITORA {
        int id_editora PK
        string nome
        string cnpj
        string site
    }

    LIVRO {
        int id_livro PK
        string nome
        string isbn
        int paginas
        int id_editora FK
    }

    LIVRO_AUTOR {
        int id_livro PK
        int id_autor PK
    }

    AUTOR {
        int id_autor PK
        string nome
        string cpf
        string rede_social
    }
