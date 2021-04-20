# QuickLookBug
Example project to show QuickLook scroll/select bug

This is a default document based application that can open plain text files with `.exampletext` extension (document identifier: `com.example.plain-text`)

We implemented a demonstration QuickLook extension that shows a bundled PDF file in a PDFView.

The extension can be tested running the QuickLookExt target. `qlmanage` will be launched and attached to the debugger. `qlmanage` will try to open a file located at : `~/Desktop/QL.exampletext`.
Project contains a simple `QL.exampletext` that can be used.

## Steps to reproduce

1) Copy `QL.exampletext` on Desktop
2) Run target `QuickLookExt`
3) You will see a QuickLook preview window showing a PDF
4) Try to scroll dragging the scrollbar or selecting text. It is not possible.
