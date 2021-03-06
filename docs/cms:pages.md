# cms:pages
Outputs a unordered list of pages.

## Usage
  <?
    $home_page = Cms_Page::create()->find_by_url('/');

    $this->render_partial('cms:pages', array(
      'list' => array_merge(array($home_page), $home_page->navigation_subpages()),
      'parent_list_class' => 'pages',
      'item_default_class' => 'item'
    ));
  ?>

## Options
### return_output
> type: `bool`  
> default: `false`

*Currently does nothing.*

---

### use_anchor_classes
> type: `bool`  
> default: `false`

*If `true`, it will output any specified anchor classes.*

---

'anchor_default_class' => ''

'anchor_current_class' => 'current'

'anchor_first_class' => 'first'

'anchor_last_class' => 'last'

'use_item_classes' => true

'item_default_class' => ''

'item_current_class' => 'current'

'item_first_class' => 'first'

'item_last_class' => 'last'

'show_item_children' => false

'item_delimiter' => '|'

'show_item_delimiter' => false

'use_list_classes' => true

'parent_page' => null

'parent_list_class' => ''

'parent_list_id' => ''

'child_list_class' => ''

'insert_before' => null

'insert_after' => null

'render_before' => null

'render_after' => null

'list' => array()
