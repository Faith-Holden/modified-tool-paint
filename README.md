# modified-tool-paint
My solution for Chapter 13 Exercise 3 of “Introduction to Programming Using Java”.
Implementation notes: This modification of ToolPaint.java adds functionality to undo
one step, have stroked-filled rects and stroke-filled ovals, and use translucent versions
of the colors for both strokes and fills.

NOTE: This is a javafx program. It requires the javafx library as a dependency. (See bottom of this README for javafx instructions).

Problem Description:
Improve the program ToolPaint.java, from Section 13.2. You can any improvements you
like, but here are some suggestions:
• Have separate menus for “Fill Color” and “Stroke Color”.
• Make it possible for the user to draw shapes that are both filled and stroked. For
example, add two new tools, “Stroked Filled Rect” and “StrokedFilledOval”.
• Add a “Line Width” menu.
• Add keyboard accelerators for some commands (see Subsection 13.5.4).
• Make it possible to use a translucent fill color. A simple approach to this is to use a
CheckMenuItem to select either fully opaque or 50% opaque fill. I don’t advise trying
to implement translucent stroke colors, since that’s more difficult.
• Add an “Undo” command that will restore the image to what it was before the last
time it was modified. This can be implemented by making a copy of the image before
you modify it. It’s possible to have a multi-level undo, but that’s harder and uses
more memory.
Remember that the ToolPaint program requires SimpleDialogs.java.

Javafx setup instructions:
Download javafx from: https://gluonhq.com/products/javafx/ (I used javafx 12). Save it to a location of your choice.
Unpack the zip folder.
Open my project with your IDE of choice (I use intellij IDEA).
Add the javafx/lib folder as an external library for the project. For intellij, this means going to "project structure" -> "libraries" -> "add library" ->{javafx location}/lib
Add the following as a VM argument for the project: --module-path "{full path to your javafx/lib folder}" --add-modules javafx.controls,javafx.fxml,javafx.base,javafx.graphics,javafx.media,javafx.swing,javafx.web
Build and run the project as normal.
