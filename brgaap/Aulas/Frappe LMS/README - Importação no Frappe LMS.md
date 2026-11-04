# Importação no Frappe LMS — NBC TG Estrutura Conceitual

## Pacote recomendado

Use **[[NBC TG Estrutura Conceitual - Frappe LMS.zip|NBC TG Estrutura Conceitual - Frappe LMS.zip]]** no Frappe Learning em **Courses → Create → Import via ZIP**. O pacote segue o formato de exportação/importação do Frappe LMS atual:

```text
course.json
chapters/*.json
lessons/*.json
```

O ZIP contém um curso, um capítulo e uma lição longa de 2h30. O corpo foi transportado em Markdown e também em um bloco Editor.js `markdown`, formato reconhecido pelas versões atuais do Frappe Learning.

### Antes de importar

- O pacote usa `Administrator` como instrutor técnico para não depender de um e-mail específico. Depois da importação, substitua pelo usuário docente correto, se necessário.
- O curso está como **não publicado** (`published: 0`), permitindo revisão antes de disponibilizá-lo aos alunos.
- Não há vídeos, imagens, SCORM ou arquivos externos no pacote.
- A aula contém referências ao CFC e ao CPC, mas o PDF oficial continua no vault Obsidian e não é embutido no ZIP.

## CSV de metadados

O arquivo **[[NBC TG Estrutura Conceitual - Curso.csv|NBC TG Estrutura Conceitual - Curso.csv]]** serve para **Courses → Import Course**. Ele importa somente os metadados do curso. Segundo a documentação oficial, o CSV não importa capítulos nem lições; para o conteúdo completo, use o ZIP.

Se o Frappe exigir o e-mail do instrutor, substitua `Administrator` pelo e-mail do usuário que terá a função de instrutor antes do upload.

## Sequência sugerida

1. Importe o ZIP.
2. Abra o curso como moderador/autor.
3. Troque `Administrator` pelo docente responsável.
4. Revise a renderização dos blocos Markdown e dos diagramas Mermaid.
5. Ajuste a política de publicação e autoinscrição.
6. Publique somente após validar as referências normativas.

## Fontes do formato

- [Documentação Frappe Learning — Create a Course](https://docs.frappe.io/learning/create-a-course)
- [Documentação Frappe Learning — Duplicating a Course](https://docs.frappe.io/learning/course-creation/duplicating-a-course)
