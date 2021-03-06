--- 
mate: |-
  NAVIGATING:
  Command-Control-T        Find Command
  Command-T                Find file in project by name (type name or acronym for file)
  Command-Shift-T          Go to Symbol
  Command-1 / 2 / etc      Switch to that number tab in Text
  Command-F2               Toggle Bookmark
  F2                       Cycle Bookmarks
  F1                       Toggle Fold
  Ctrl-Shift-T             Show TODO List
  
  SELECTING:
  Control-W                Select current word
  Command-Shift-L          Select current line
  Command-Shift-B          Select enclosed braces
  Command-Control-B        Select current scope
  
  EDITING:
  Escape                   Tab completion of variables / strings
  Command-Enter            Go to end of line and return
  Command-Shift-V          Paste previous item in clipboard history
  Command-Control-Alt-V    Select from Clipboard
  Command-Alt-A            Edit Multiple Lines
  Control-U                Upcase
  Control-Shift-U          Downcase
  Control-Alt-U            TitleCase
  Control-Alt-Q            Unwrap line, remove newlines
  Control-K                Kill all text to end of line
  Control-Y                Yank back all text from kill
  Control-D                Delete character (not backspace)
  
  SEARCH & REPLACE:
  Control-S                Live Search / Find Next
  Control-Shift-S          Find Previous
  Command-F                Find
  Command-Shift-F          Find in Project
  
  COMMENTING, QUOTING, AND INDENTING:
  Command-/                Comment Toggle
  Control-"                Single/Double Quotes Toggle
  Command-]                Indent Selection
  Command-[                Un-indent Selection
  Command-Alt-[            Reindent
  
  CTAGS:
  Control-]                Lookup Definition
  Command-Control-B        Source Browser
  
  WEB:
  Command-Control-Alt-P    Web Preview
  Command-Control-Shift-W  Update missing tags for all lines
  Control-Shift-<          Create tags        (HTML)
  Control-Enter            <br/>
  Control-Shift-L          Wrap selection as Link
  doctype-Tab              Document Type Section
  head-Tab          
  body-Tab
  table-Tab
  Command-&                Menu for URL
  Command-Shift-C          Edit Hex Color with Color Picker
  
  COMMAND LINE:
  find {app,lib} -name '*.rb' -o -name '*.rhtml' -print0 | xargs -0 mate
  
  RUBY:
  Control-H                Documentation for word
  Control-{                Toggle do/end {/}
  Control-|                Install Plugin, Dump DB, etc. Menu
  %                        Eval as Ruby (not in output)
  Command-R                Run Ruby Script
  Control-Shift-E          Execute Line as Ruby
  Control-Shift-Command-E  Execute all lines marked with '# =>' as Ruby
  R-Tab                    attr_reader
  W-Tab                    attr_writer
  RW-Tab                   attr_accessor 
  def-Tab                  define method
  if-Tab                   if... end
  case-Tab                 case...when...end
  cla-Tab                  Menu for different types of classes
  mod-Tab                  Menu for different types of modules
  ea-Tab                   each { |e|  }
  eawi-Tab                 each_with_index { |e, i|  }
  
  RAILS MIGRATIONS:
  mccc-Tab                 Create Several Columns
  mcol-Tab                 Column Menu
  mtab-Tab                 Table Menu
  
  RAILS VIEWS:
  Control-Shift-V          <%= %> Insert (and Toggle)
  Control-Shift-H          Create partial from selection
  
  RAILS CONTROLLERS:
  Control-P                params
  Control-J                session
  Command-Shift-Alt-Down   Jump to controller helper/test/view/etc.
  
  SUBVERSION:
  Control-Shift-A          SVN Menu
    1                      Add
    2                      Remove
    3                      Revert
    5                      Commit
    6                      Blame
    7                      Info
    8                      Log
    9                      View Revision
    0                      Stat
  
  SHELL:
  Contol-R                 Run Current Line in the Shell
