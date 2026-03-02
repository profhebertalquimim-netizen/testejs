```mermaid
erDiagram
    EDITORA {
        int id_editora PK
        string nome
    }
    LIVRO {
        int id_livro PK
        string nome
        int id_editora FK
    }
    EDITORA ||--o{ LIVRO : publica
