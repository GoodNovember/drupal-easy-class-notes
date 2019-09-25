Paragaphs
  They are fieldable entities
  They are per node, not entity type or bundle.

Paragraph Types
  They are predefined layouts.

Page Managaer acts as a Dispatcher for custom paths.
  It works well with Panels.

Page Manager can return different results depending on various rules.
  May have different results for example:
    /home
      -- home for authenticated users
      -- home for anon users
      -- home for specific authenticated users

Page Manager Varient often returns a Panel Layout.
  Other things it can do:
    HTTP status codes.
    Block Pages
  With panels instaled:
    Panel

Panels module:
  - Layouts for page manager paths
  - Override existing drupal destinations. (Layout builder does this too.)

Panels Layouts:
  - "Layout Discovery" -- enables modules to provide more layouts for Layout Builder.
  - Examples:
    - Radix Layouts
    - Bootstrap Layouts

