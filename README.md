# SpeedEq
    SpeedEq is a small MS Word addin used to simplify the
    insertion of equations and cross-references in MS Word. It
    offers:

    - One mouse click to insert and position an equation and its
      sequence number using definable patterns;

    - Three mouse clicks to insert a corss reference to an
      equation;

    - Dynamic sequential number and reference: it means that
      sequential number associated with an equation, and all
      references to this equation are updated automatically when
      new equations are inserted, or existing equations are
      deleted or moved (Copy/Cut/Paste);

    - Start new equation series, split a series or merge two
      existing serieses;

    - Reposition existing equations and their sequential numbers
      when page / column width is changed;

    - No side effect: Equations, associated sequential numbers
      and any reference that are inserted using SpeedEq will
      display normally when SpeedEq is not available, for
      example, when the document is opened on another computer.

    - Very easy to use through its user friendly interface.

How to Install:
---------------

    Copy all files to the startup folder of the MS Word. The
    directory of this folder can be found by going to: Tools | 
    Options and click "File Locations" tab, find the item  
    "StartUp" in the list.


How are equations and sequential numbers positioned:
----------------------------------------------------

    The position etc of the equations and the sequential nubmers
    are specified using a data structure called 'Style'. It has
    the following members:

    - Equation editor: Microsoft Equation and MathType are
      commonly used equation editors;

    - Equation position: a number in the range of 0.0 (left most)
      and 1.0 (right most);

    - Equation alignment: left, middle or right;

    - Seq number position (0.0 to 1.0);

    - Seq number alignment (left, middle or right);

    - Seq number prefix and suffix, and internal prefix and
      suffix: any string attached to the sequential number. The 
      whole sequence will appear as: 
      
      <Prefix><Internal Prefix><number><Internal suffix><Suffix>

      For example, if the four parts are: "(", "A", "", ")" where
      the internal suffix is empty, the whole sequence is then: 
      "(A5)" where 5 is the automatic sequential number.

      The internal prefix and suffix, together with the seq number
      appear in references to this equation.

    - Reference prefix and suffix: any strings attached to the
      cross reference. The whole reference will appear as: 

      <Prefix><Seq number + internal prefix & suffix><Suffix>

      For example, if the two parts are: "Eq(" and ")", the whole 
      reference will be: "Eq(A5)" where "A5" come from sequential
      number.


    SpeedEq provides a default style, which is defined as:

      - Eq Editor:            Microsoft Equation;
      - Eq position:          0.5, or middle of the line;
      - Eq alignment:         middle;
      - Seq number position:  1.0, or right of the line;
      - Seq number alignment: right;
      - Seq number prefix:    '(';
      - Seq number suffix:    ')';
      - Internal prefix:      "" or empty;
      - Internal suffix:      "" or empty;
      - Ref prefix:           'Eq(';
      - Ref suffix:           ')'.

    It is possible to define other styles or change existing
    styles. User interfaces have been provided to manage styles.

    New styles are saved in the system registry when they are
    initially defined. When a style is used in a document, it
    will also be saved with that document so that the information
    is available when the document is moved to other computers.

How to Use SpeedEq:
-------------------

    It is rather straight forward to use SpeedEq. If SpeeqEq is
    installed succefully, a tool bar will be created when MS Word
    is started.

    - To insert an equation using current style:

        Click the [Insert] button: a sequential number will be
        inserted, and the equation editor will be opened, either
        as a stand alone window, or an in-place box. Edit the
        equation and exit the equation editor.

    - To insert an equation of other styles:

        Click the down arror beside the [Insert] button, a list
        of all available styles will drop down. Chose the style
        you want to use. A equation will be inserted using this
        style, which at the mean time becomes the current style.

    - To insert a reference to an equation:

        Click the [Reference] button, a dialog will show up.
        Select the equation from the list in the dialog box and
        press <Enter> or click [OK]. To preview an equation,
        select it and press <Space> or click the [See It]. The
        Document will be scrolled to the position of the selected
        equation and the line containing the equation will be
        highlighted.

    - To start a new series or split an series:

        Insert the first equation of the new series, if not yet.
        Put the insertion cursor (caret) on the line containing
        the equation and click [More | New Series].

    - To merge two series:

        Put the insertion cursor (caret) on the line containing
        the first equation of the second series, and click
        [More | Merge Series].

    - To delete an equation:

        You can simply delte it but it is recommended to use the
        [Delete] button.

    - To reposition equations and sequence number:

        When the width of the page / column is changed, or the
        number of column is changed, you can click [Refresh] to
        adjust the position of equations and their sequence
        numbers.

        This button also performs an update of all fields in the
        document. If some sequential number appear incorrect. Use
        this button will solve the problem.

    - To define new styles, or change existing styles:

        Click [More | Manage Styles]. You can add new style to or
        delete a style from the global style list. You can edit
        styles in both lists.

        SpeedEq add a style to the document specific style list
        when the style is used the first time. You can also click
        [Cleanup] button to remove those styles that are no
        longer used in the document.

        Styles in the document specific list can be copied to the
        global list so the styles are made available to other
        documents.

    - Options: a few options are available 

        * Auto Refresh: automatically refresh the equations when
          equations are inserted or deleted, and so on;

        * Asign short cut key: assign short cut key to commands 
          when startup;  

        * Put equation in new paragraph: if this options is checked,
          an equation will be inserted into a new paragraph, 
          otherwise the equation will remain in the current paragraph.

    - Ohter commands in the "More" menu:

        * Show / Hide Bookmarks: turn on / off Bookmark & field 
          highlighting;

        * Restart: use it if SpeedEq is not working properly in anyway;


Tips:
-----

    - To move a equation, select the whole line and cut + Paste. 
      References to this equation will be maintained properly, 
      sequential number will be updated automatically (if not, 
      click [Refresh]). Drag & Drop can also be used to move an
      equation, but the whole line must be moved;

    
