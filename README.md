# QuickLookBug
Example project to show QuickLook scroll/select bug on *Big Sur*

On *Catalina* and below, everything works fine and it is possible to select PDF text and to drag the PDF scrollbar with the mouse.

On *Big Sur* clicks on the PDFView seem to be intercepted by an invisible superview/layer. It is not possible to select text nor to move the scrollbar. Every mouse drag just moves the whole QL window.

### Sample project
This is a default document based application that can open plain text files with `.exampletext` extension (document identifier: `com.example.plain-text`)

We implemented a demonstration QuickLook extension that shows a bundled PDF file in a PDFView.

The extension can be tested running the QuickLookExt target. `qlmanage` will be launched and attached to the debugger. `qlmanage` will try to open a file located at : `~/Desktop/QL.exampletext`.
Project contains a simple `QL.exampletext` that can be used.

### Steps to reproduce

1) Copy `QL.exampletext` on Desktop
2) Run target `QuickLookExt`
3) You will see a QuickLook preview window showing a PDF
4) Try to scroll dragging the scrollbar or selecting text. It is not possible.
